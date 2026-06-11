# UAIV-Foundry `.io` 轻量项目页包

更新时间：2026-06-11

## 目的

这个目录用于先搭建一个轻量 `.io` 项目页，让老师、合作者或标注团队快速理解：

- UAIV-Foundry 是什么；
- 它和 UAIV-Real、UAIV-Labeler 的关系；
- 当前首发城市治理数据做到哪一步；
- 为什么 Foundry 不是普通资源库，也不是另一个标注平台；
- 后续人工标注、QA、发布和 benchmark 如何进入闭环。

## 文件

| 文件 | 说明 |
| --- | --- |
| `index.html` | 自包含中文首页，可直接部署到 GitHub Pages |
| `README.md` | 本说明 |
| `DEPLOYMENT.md` | 上传到 `.io` 的操作步骤 |

## 当前定位

这是：

```text
pre-release engineering project page
```

不是：

```text
final UAIV-Real public release page
```

页面中已经明确写明：

- 数据尚未正式公开；
- reviewed annotations 尚未完成；
- final QA 尚未完成；
- public links 尚未确定；
- real benchmark 尚未完成。

## 推荐使用方式

当前不急着上传完整 `UAIV-Foundry` 工程仓库，可以先只上传本目录内容到：

```text
JennyZhang0810.github.io
```

或一个单独的 GitHub Pages 仓库，例如：

```text
uaiv-foundry-page
```

这样公开展示更干净，不会把内部日志、脚本草稿、过程文档全部暴露出来。
