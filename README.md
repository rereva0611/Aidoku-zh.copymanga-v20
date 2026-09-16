# 拷贝漫画 Plus

这是一个为 Aidoku 提供拷贝漫画阅读功能的独立 Source。

本项目基于已合并至 Aidoku Community 的 `zh.copymanga` v20 源码整理发布，个人仓库主要用于源码查看和 `.aix` 文件下载。

- Source ID：`zh.copymanga`
- 当前版本：`v20`
- 默认网址：`https://www.copy5000.com`

## 安装

1. 在本项目的 Releases 页面下载 `zh.copymanga-v20.aix`。
2. 在设备上使用 Aidoku 打开该 `.aix` 文件。
3. 确认安装后，在 Aidoku 的图源列表中使用拷贝漫画。

## Aidoku中文使用教程

`https://github.com/rereva0611/aidoku-guide-zh`

## 功能

- 搜索漫画和使用标签筛选；
- 浏览网站的“全新上架”内容；
- 登录后查看“我的收藏”；
- 在详情页打开评论区；
- 在详情页收藏或取消收藏漫画；
- 章节按上传时间从新到旧排列；
- 支持图片画质和格式设置。

## 使用提醒

- 登录后才能查看“我的收藏”并使用收藏功能。
- 详情页的评论区和收藏按钮默认关闭，可在图源设置中手动开启。
- 已加入 Aidoku 书架的漫画，需要刷新一次详情页后，相关按钮才会显示。
- 收藏功能可能响应较慢，请不要连续点击。
- 默认网址为 `www.copy5000.com`，其他已验证网址作为备用线路。

## 免责声明

本项目与 Aidoku、CopyManga 及相关网站均无官方关联。

代码与配置文件按照 MIT OR Apache-2.0 双许可证发布。网站内容和图标等素材的权利归相应权利人所有。

若相关权利人认为仓库中的素材侵权，请通过 GitHub Issues 联系，我会及时处理。

## 从源码构建

需要安装 Rust、`wasm32-unknown-unknown` 编译目标和 Aidoku CLI。

```bash
rustup target add wasm32-unknown-unknown
aidoku package .
aidoku verify package.aix
```
