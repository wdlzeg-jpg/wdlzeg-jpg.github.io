# AI 视频替换说明

页面的视频内容集中配置在 `app/project-data.ts` 的 `videoItems` 中。

1. 将视频文件放入本目录，建议同时提供 `.webm` 与 `.mp4`。
2. 如有单独封面图，也放入本目录。
3. 在对应条目中填写公开路径，例如：

```ts
poster: "/videos/sisiful-cover.jpg",
webm: "/videos/sisiful-main.webm",
mp4: "/videos/sisiful-main.mp4",
```

未填写视频路径时，网站会自动显示现有的高完成度占位封面，不影响布局。

推荐规格：

- 主视频：16:9，1920×1080，10–20 秒，静音循环。
- 竖屏短视频：9:16，1080×1920。
- 单条文件尽量控制在 8 MB 以内。
- 保留字幕与封面，避免依赖自动播放传达关键信息。
