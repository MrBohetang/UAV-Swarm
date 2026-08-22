# 软件、数据与成果工作流

## 1. 推荐的软件学习顺序

### 第一主线：DJI Terra + QGIS

适合希望快速建立完整工程流程的初学者：

**无人机采集 → DJI Terra → 正射/点云/DSM/三维 → QGIS → 测量/标注/出图**

DJI官方目前提供 Terra 用户手册、质量报告说明和版本资料；学习时应以当前官方版本为准。

### 第二主线：WebODM + QGIS

适合想理解开源摄影测量流程的人。

WebODM可以从航拍影像生成地理参考地图、点云、高程模型和纹理三维模型，也提供地面控制点和飞行建议等文档。

### 第三主线：Agisoft Metashape

适合进一步理解摄影测量参数和多种传感器数据处理。

---

# 2. 学软件不要从“按钮”开始

每次处理数据都按下面的问题走：

1. 我的输入是什么？
2. 我要得到什么成果？
3. 哪个参数影响这个成果？
4. 输出后怎么检查质量？
5. 如果失败，可能是哪一步出了问题？

这样你不会变成“只会照着视频点按钮”。

---

# 3. 推荐数据目录

```text
project_name/
├── 00_admin/
│   ├── task.md
│   ├── risk-assessment.md
│   └── equipment.txt
├── 01_raw/
│   ├── images/
│   └── flight-log/
├── 02_check/
├── 03_processing/
├── 04_products/
│   ├── orthomosaic/
│   ├── dsm-dtm/
│   ├── pointcloud/
│   └── model/
├── 05_gis/
├── 06_inspection/
├── 07_report/
└── 09_archive/
```

---

# 4. 文件格式认知

| 格式 | 常见用途 |
|---|---|
| JPG | 航拍照片 |
| DNG/RAW | 原始影像，适合需要更大后期空间的场景 |
| GeoTIFF | 正射/DSM/栅格成果 |
| LAS/LAZ | 点云 |
| OBJ/PLY | 三维模型/点云等 |
| SHP | 传统GIS矢量数据 |
| GeoPackage | 推荐的现代GIS容器之一 |
| KML/KMZ | 地理可视化/交换 |
| CSV | 表格和属性数据 |

---

# 5. DJI Terra学习清单

## Level 1

- 安装
- 导入照片
- 创建任务
- 检查影像
- 查看重建结果
- 导出成果

## Level 2

- 航测重建参数
- 质量报告
- 坐标系统
- GCP/检查点
- 点云处理
- DSM/DTM
- 三维重建

## Level 3

- 大区域任务
- 复杂地形
- RTK/PPK数据
- 质量控制
- 参数对比实验

---

# 6. WebODM学习清单

- 安装/启动
- 创建项目
- 上传照片
- 设置任务
- 查看处理状态
- 下载正射
- 查看点云
- 研究GCP工作流
- 对比不同参数结果

官方文档说明WebODM支持生成地理参考地图、点云、高程模型和纹理三维模型，并提供GCP与飞行建议等学习内容。

---

# 7. QGIS学习清单

## Level 1：看地图

- 图层
- 栅格
- 矢量
- CRS
- 属性表

## Level 2：改地图

- 点线面
- 编辑属性
- 标注
- 分类渲染

## Level 3：分析

- 距离
- 面积
- 缓冲区
- 栅格计算
- 等高线
- 空间查询

## Level 4：交付

- 布局
- 图例
- 比例尺
- 北箭头
- 标题
- PDF/图片导出

QGIS官方提供用户指南、Training Manual和Gentle Introduction等资料；训练时优先使用官方文档。

---

# 8. 软件实验：同一组照片做三遍

这是非常重要的进阶练习。

同一批照片分别使用：

1. DJI Terra
2. WebODM
3. Metashape

记录：

- 处理时间
- 参数
- 正射质量
- 点云质量
- 空洞
- 纹理
- 输出文件大小
- 操作难度

最后写一页《三种软件处理结果对比》。

你会从“会软件”升级到“懂摄影测量流程”。

---

# 9. 推荐官方资料

- DJI Terra下载与用户手册： https://www.dji.com/downloads/products/dji-terra
- DJI Enterprise Terra： https://enterprise.dji.com/dji-terra/downloads
- QGIS资源中心： https://www.qgis.org/resources/hub/
- QGIS中文培训手册： https://docs.qgis.org/3.44/zh-Hans/docs/training_manual/index.html
- WebODM文档： https://docs.webodm.org/
- Agisoft Metashape手册： https://www.agisoft.com/pdf/metashape-pro_2_0_en.pdf

# 10. 版本意识

软件会持续更新，因此不要把教程里的某个按钮位置当成永恒知识。

学习重点应该是：

**数据 → 原理 → 参数 → 结果 → 质量检查。**

界面变化后，只要这条逻辑没有丢，你依然能够重新找到功能。
