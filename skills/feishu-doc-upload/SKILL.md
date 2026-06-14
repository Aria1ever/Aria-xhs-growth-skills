---
name: feishu-doc-upload
description: 把当前对话输出的文案、方案或内容传到飞书文档。当用户对输出内容满意、说"传飞书""存到文档""发到飞书""帮我存起来"时使用。支持新建文档和追加到已有文档两种模式。需要本地已安装 feishu-cli 并完成登录。触发词：传飞书、存飞书、发到飞书文档、帮我存起来、传上去、存文档。
---

# 飞书文档上传

把对话中已定稿的内容写入飞书文档，省去手动复制粘贴。

## 前置检查

上传前先确认 feishu-cli 已登录：

```bash
feishu-cli auth status
```

未登录则提示用户运行：

```bash
feishu-cli auth login --recommend
```

登录后回来继续。

---

## 上传流程

### Step 1：确认目标

问用户一句：

> "新建一个飞书文档，还是追加到已有文档？如果是已有文档，请把链接发给我。"

### Step 2：整理内容为 Markdown

把当前对话里定稿的内容整理好，写入临时文件：

```bash
TMPFILE=$(mktemp /tmp/feishu_upload_XXXXXX.md)
cat > "$TMPFILE" << 'EOF'
# [内容标题]

[正文]

[话题标签]
EOF
```

### Step 3：上传

**新建文档：**

```bash
feishu-cli doc import "$TMPFILE" --title "[内容标题]"
```

**追加到已有文档：**

从用户提供的链接中提取 document_id（链接格式：`https://xxx.feishu.cn/docx/<document_id>`）

```bash
feishu-cli doc content-update <document_id> --mode append --markdown-file "$TMPFILE"
```

### Step 4：收尾

上传成功后把文档链接告知用户，删除临时文件：

```bash
rm -f "$TMPFILE"
```

---

## 依赖说明

本 skill 依赖 [feishu-cli](https://github.com/riba2534/feishu-cli)，首次使用需要安装：

```bash
gh repo clone riba2534/feishu-cli
```

按 feishu-cli 的 README 完成安装和初始配置后，运行 `feishu-cli auth login --recommend` 完成登录，即可使用本 skill。
