# UAIV-Foundry `.io` 项目页部署说明

更新时间：2026-06-11

## 推荐方案

当前建议先上传轻量项目页，而不是完整 `UAIV-Foundry` 仓库。

原因：

- 完整仓库后续还会大量修改；
- 完整仓库包含内部日志、过程文档、脚本草稿和生成图草稿；
- 现在更需要一个清晰页面，让别人先理解 Foundry 是什么；
- 数据尚未正式公开，完整仓库不宜被误解为 final release。

## 需要上传的文件

只上传这个目录里的 3 个文件：

```text
index.html
README.md
DEPLOYMENT.md
```

本目录路径：

```text
UAIV-Foundry/docs/io_site_package
```

## 方案 A：上传到个人主页仓库

适合想要一个主站入口：

```text
https://JennyZhang0810.github.io
```

### 1. 在 GitHub 创建仓库

仓库名必须是：

```text
JennyZhang0810.github.io
```

建议不要勾选 README / .gitignore / license。

### 2. 在本地 Git Bash 操作

把 `io_site_package` 复制到 Windows 本地任意位置，例如：

```text
D:\UAIV-Foundry-io
```

进入目录：

```bash
cd /d D:\UAIV-Foundry-io
```

初始化并上传：

```bash
git init
git branch -M main
git add .
git commit -m "Initial UAIV-Foundry project page"
git remote add origin https://github.com/JennyZhang0810/JennyZhang0810.github.io.git
git push -u origin main
```

### 3. 打开页面

稍等 1-3 分钟后访问：

```text
https://JennyZhang0810.github.io
```

## 方案 B：上传到单独项目页仓库

适合不占用个人主页，只做 Foundry 项目页：

```text
https://JennyZhang0810.github.io/uaiv-foundry
```

### 1. 在 GitHub 创建仓库

例如：

```text
uaiv-foundry
```

或：

```text
uaiv-foundry-page
```

### 2. 上传文件

```bash
cd /d D:\UAIV-Foundry-io
git init
git branch -M main
git add .
git commit -m "Initial UAIV-Foundry project page"
git remote add origin https://github.com/JennyZhang0810/uaiv-foundry.git
git push -u origin main
```

### 3. 打开 GitHub Pages

进入 GitHub 仓库页面：

```text
Settings -> Pages
```

选择：

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

保存后访问：

```text
https://JennyZhang0810.github.io/uaiv-foundry
```

## 后续如何更新页面

每次我改完 `index.html` 后，你只需要把新的 `index.html` 覆盖到本地页面仓库，然后：

```bash
git status
git add index.html
git commit -m "Update UAIV-Foundry project page"
git push
```

如果 README 或部署说明也改了：

```bash
git add .
git commit -m "Update UAIV-Foundry page docs"
git push
```

## 当前页面不能写什么

不要写：

```text
UAIV-Real has been publicly released
Final QA passed
Real benchmark results are available
All annotations are reviewed
```

当前只能写：

```text
pre-release engineering preview
Golden/full annotation pending
release pending
benchmark dry-run ready
```

## 后续可迭代方向

1. 加入更好的 Foundry 架构图。
2. 加入 Golden 标注完成后的真实 QA 数字。
3. 加入首发数据图像样例，但必须确认可公开展示。
4. 加入最终 dataset card 和 public download links。
5. 数据公开后，再把页面从 preview 改成 official release page。
