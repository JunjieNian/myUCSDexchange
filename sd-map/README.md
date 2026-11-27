# 圣迭戈游记地图

地图通过游记里的地图链接嵌入个人网站第三章。景点坐标、简介和行程在 [places.json](places.json)；[transit.json](transit.json) 保存从 [SanGIS](https://data.sandiego.gov/datasets/gis-transit-routes/) 线路数据裁出的乘车区间，键为 `线路:上车站:下车站`。页面提供单独的班次查询链接。

添加照片时，把 JPEG、PNG、WebP 或 AVIF 文件放到 `sd-map/photos/`，再给对应景点添加 `photo`。例如 Black’s Beach 可以在 `places.json` 中写 `"photo": {"src": "photos/blacks-beach.jpg", "alt": "从悬崖步道看 Black’s Beach"}`。文件名大小写需一致。照片更新随游记同步到网站。
