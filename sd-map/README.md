# 圣迭戈游记地图

地图通过游记里的地图链接嵌入个人网站第三章。景点坐标、简介和行程在 [places.json](places.json)；[transit.json](transit.json) 保存从 [SanGIS](https://data.sandiego.gov/datasets/gis-transit-routes/) 线路数据裁出的乘车区间，键为 `线路:上车站:下车站`。页面提供单独的班次查询链接。

把 JPEG、PNG、WebP 或 AVIF 文件放进 `sd-map/photos/`，在 `places.json` 对应的景点里按展示顺序列出 `photos`。每项包含 `src`，也可以加 `alt` 描述照片内容。文件名大小写需一致。留空的景点会显示「暂无照片」。推送到 `main` 后，地图和照片会同步到网站。

```json
"photos": [
  {"src": "photos/BlacksBeach1.jpg"},
  {"src": "photos/BlacksBeach2.jpg"}
]
```
