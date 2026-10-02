# City Data Visual

[English](README.md) · **中文**

以手机竖屏（`1080×1920`）为主的数据可视化作品集，题材涵盖城市空间、人口、地形水文、气候与文化地理，形式包括静态图、预渲染动画与三维场景。署名 **@一尺之棰 / Zeno.yczc**。

> 本仓库只发布成图与简短说明。渲染代码、研究笔记、参数合同、原始数据与中间产物保留在本地（见[仓库范围](#仓库范围)）。

## 作品展示

### 城市建成空间时间线

基于 CMAB v7 / GAIA 派生的建成空间首次出现数据，为十二座中国城市制作逐年时间线。

| 北京 | 上海 | 深圳 | 长沙 | 广州 | 南京 |
|---|---|---|---|---|---|
| <img src="public-works/building-age/beijing-2024.webp" width="130" alt="北京建成空间时间线"> | <img src="public-works/building-age/shanghai-2018.webp" width="130" alt="上海建成空间时间线"> | <img src="public-works/building-age/shenzhen-2018.webp" width="130" alt="深圳建成空间时间线"> | <img src="public-works/building-age/changsha-2024.webp" width="130" alt="长沙建成空间时间线"> | <img src="public-works/building-age/guangzhou-2024.webp" width="130" alt="广州建成空间时间线"> | <img src="public-works/building-age/nanjing-2018.webp" width="130" alt="南京建成空间时间线"> |

| 杭州 | 西安 | 成都 | 拉萨 | 郑州 | 沈阳 |
|---|---|---|---|---|---|
| <img src="public-works/building-age/hangzhou-2024.webp" width="130" alt="杭州建成空间时间线"> | <img src="public-works/building-age/xian-2024.webp" width="130" alt="西安建成空间时间线"> | <img src="public-works/building-age/chengdu-2024.webp" width="130" alt="成都建成空间时间线"> | <img src="public-works/building-age/lhasa-2024.webp" width="130" alt="拉萨建成空间时间线"> | <img src="public-works/building-age/zhengzhou-2024.webp" width="130" alt="郑州建成空间时间线"> | <img src="public-works/building-age/shenyang-2024.webp" width="130" alt="沈阳建成空间时间线"> |

`Age` 是 GAIA 派生的不透水面首次出现代理指标，**不是**官方建筑竣工年份。

### 人口、气候与夜间灯光

| 中国人口 H3 场 | 广州人口 H3 场 | 2023 中国雷季 | 2024 东亚灯火 |
|---|---|---|---|
| <img src="public-works/population-3d/china-national.png" width="180" alt="中国人口 H3 三维场"> | <img src="public-works/population-3d/guangzhou.png" width="180" alt="广州人口 H3 三维场"> | <img src="public-works/lightning/china-lightning-season-2023.webp" width="180" alt="2023 中国雷季"> | <img src="public-works/nightlights/east-asia-2024.webp" width="180" alt="2024 东亚夜间灯光"> |

### 地形与水文

| 中国方言地形 | 长江水文地形 | 长江人口密度 | 台湾西部水系 | 大连 GIS 地形 | 吉隆口岸地形 |
|---|---|---|---|---|---|
| <img src="public-works/dialect/chinese-dialect-relief.png" width="130" alt="中国方言地形图"> | <img src="public-works/watershed/02-hydrology-color.png" width="130" alt="长江水文地形"> | <img src="public-works/watershed/03-population-density.png" width="130" alt="长江流域人口密度"> | <img src="public-works/watershed/taiwan-hydrology.webp" width="130" alt="台湾水系"> | <img src="public-works/terrain/dalian-gis-relief.webp" width="130" alt="大连 GIS 地形"> | <img src="public-works/gyirong/gyirong-port-terrain.png" width="130" alt="吉隆口岸地形"> |

### 人口统计与科普

| 尚未成家（普查） | 2023 世界新生儿 | 死亡概率 | 把地球摊平 | 英语与世界 | 世界怎么叫"中国" |
|---|---|---|---|---|---|
| <img src="public-works/census/china-marriage-census-2020.webp" width="130" alt="2020 普查未婚年龄分布"> | <img src="public-works/world-births/world-births-2023.webp" width="130" alt="2023 世界出生人口"> | <img src="public-works/explainers/life-expectancy-probability.webp" width="130" alt="预期寿命科普"> | <img src="public-works/explainers/map-projection-equal-earth.webp" width="130" alt="地图投影科普"> | <img src="public-works/explainers/english-in-the-world.webp" width="130" alt="英语与世界"> | <img src="public-works/explainers/names-for-china.webp" width="130" alt="中国的外语名称"> |

### 动画截帧、算法与三维概念

| 2026 月相日历 | 台湾灯塔与航标 | 上海最短路径 | 粒子转场 | 大观园（WebGPU） |
|---|---|---|---|---|
| <img src="public-works/motion-stills/moon-calendar-2026.webp" width="150" alt="月相日历动画截帧"> | <img src="public-works/motion-stills/taiwan-coastal-lights.webp" width="150" alt="台湾灯塔动画截帧"> | <img src="public-works/route-search/shanghai-dijkstra.webp" width="150" alt="上海 Dijkstra 路径搜索"> | <img src="public-works/particle-morph/dalian-source.png" width="150" alt="大连到广州粒子转场"> | <img src="public-works/concept/daguanyuan-yihongyuan.webp" width="150" alt="大观园怡红院 WebGPU 概念"> |

完整文件清单见 [PUBLIC_WORKS_MANIFEST.md](PUBLIC_WORKS_MANIFEST.md)。

## 数据可视化能力总结

### 数据源

| 领域 | 数据源 | 应用作品 |
|---|---|---|
| 建成环境 | CMAB v7（GAIA 派生不透水面首次出现） | 城市建成空间时间线 |
| 人口 | Kontur Population 2023（H3 第 8 级，约 400 m）；2000 / 2010 / 2020 年人口普查；联合国《世界人口展望 2024》 | 人口 H3 场、长江 / 台湾人口密度、未婚普查图、世界新生儿 |
| 地形与地表覆盖 | Mapzen Terrarium 高程瓦片、SRTM、ESA WorldCover、卫星影像 | 方言地形、长江、台湾、大连、吉隆 |
| 水文 | HydroSHEDS（HydroRIVERS、HydroBASINS）；台湾水利署河川分区 | 长江与台湾西部水系 |
| 大气与夜光 | 风云四号 A 星闪电成像仪（FY-4A LMI）；VIIRS 夜间灯光 VNL 2024；NASA Blue Marble；Meteostat | 中国雷季、东亚灯火、上海气温 |
| 边界与网络 | GADM、Natural Earth、OpenStreetMap（Overpass）、NGA 灯标表 | 底图、路网搜索、灯塔动画 |
| 天文 | JPL DE421 星历（Skyfield） | 2026 月相日历 |
| 人文与语言 | CBDB 中国历代人物传记资料库、开放方言数据、历史沿革资料、世界银行 / Ethnologue 语言统计 | 唐代诗人关系、方言地形、边界历史、英语与世界 |

### 方法

- **制图**：默认使用等积投影（中国用 GRS80 阿尔伯斯等积，全球用 Equal Earth），以投影合同保证栅格底图与矢量 / 柱体图层严格对齐。
- **空间聚合**：直接使用原生 H3 六边形格网（不重采样、不做核密度平滑）；事件点按等积网格累计（如雷电 8 km 网格）；流域与县级剖面。
- **地形与三维**：DEM 晕渲合成并保留主题色相；Blender Cycles 制作地形、人口柱、夜光与海岸灯光动画；Three.js WebGPU 程序化场景。
- **动效**：确定性 Canvas 粒子系统、预渲染 WebP 帧序列、可任意跳转的时间轴，经 FFmpeg 输出 H.264。
- **算法可视化**：在真实 OpenStreetMap 路网（NetworkX）上回放 Dijkstra、A*、双向与贪心搜索，按真实事件顺序而非模拟进度。
- **科普图解**：为死亡概率、预期寿命面积等概念使用明确标注的构造示例数据。

### 工具链

Python（GeoPandas、rasterio、pyproj、h3、NetworkX、Pillow、matplotlib）· Node.js（sharp、Playwright）· d3-geo · HTML Canvas · Three.js / WebGPU · Blender（Cycles）· FFmpeg

### 核验规范

- 每个 GIS 输入在渲染前检查许可、坐标系、要素 / 像元数量、字段、数值分布、空间覆盖与时间语义。
- 数据清单记录版本与 SHA-256；已发布系列用冻结的视觉合同锁定配色、投影、相机与排版。
- 成品经 `ffprobe`、完整解码与解码帧检查，排查裁切、文字碰撞、空白帧与地图错位。
- 语义表述如实：代理指标不冒充官方统计，模型推算时段明确标注，镜头窗口内的格网合计绝不当作城市官方人口。

## 仓库范围

- 公开内容：`public-works/` 下的成图、本 README、作品清单与 [`CLAUDE.md`](CLAUDE.md)。
- 仅保留在本地：渲染器、研究笔记、合同、第三方原始数据、Blender 场景、逐帧与视频。根目录 `.gitignore` 采用白名单，未经显式添加的内容不会提交。
- 2026-09 新增的图片为本地定稿的 WebP 网页版副本；此前的图片为未改动原图。

## 地图与数据声明

部分全国地图中的九段线仅作显示几何，不参与面积、粒子或统计计算，且不是经出版审核的官方地图素材。第三方数据、地图图层、字体与影像仍受其原始许可与署名要求约束。

## 授权

`public-works/` 中的图片与本仓库文字 © Felix Liu（@一尺之棰 / Zeno.yczc），以 [CC BY-NC 4.0](LICENSE) 授权：可非商业转载和改编，须注明出处。第三方数据与地图图层仍按上文所述的原始许可执行。
