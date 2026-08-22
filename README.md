# UAV-Swarm

> 无人机技术学习仓库：从无人机编队方向转向 **无人机测绘 + 无人机巡检 + 飞行操控** 的系统学习。

## 当前学习主线

本仓库当前以零基础学习者为对象，目标不是先学编程，而是先形成一条完整的无人机作业能力链：

**安全飞行 → 手动操控 → 航线规划 → 航测采集 → 建图建模 → GIS处理 → 巡检采集 → 缺陷判读 → 报告交付 → 项目复盘**

编队/无人机集群编程暂时放到后续选修，不作为当前主线。

## 学习资料

- [01 从零到精通路线图](survey-inspection/01-roadmap.md)
- [02 零基础文字教程](survey-inspection/02-zero-to-one-manual.md)
- [03 视频课程脚本与拍摄清单](survey-inspection/03-video-course.md)
- [04 实践教学用例与项目制训练](survey-inspection/04-practice-projects.md)
- [05 飞行安全与作业检查清单](survey-inspection/05-flight-and-safety-checklists.md)
- [06 软件、数据与成果工作流](survey-inspection/06-software-and-data-workflow.md)
- [07 学习成果、作品集与就业路线](survey-inspection/07-portfolio-and-career.md)

## 推荐学习顺序

1. 先完成安全、法规、遥控器/飞控基础。
2. 用小型无人机练手动悬停、定点、航向、矩形航线。
3. 学会任务规划和影像质量控制。
4. 用真实航测照片完成正射、DSM/DTM、点云、三维模型。
5. 学 QGIS，学会把成果变成可量测、可标注、可出图的 GIS 数据。
6. 进入巡检：构件识别、拍摄构图、缺陷分类、复核和报告。
7. 最后做综合项目，把飞行、数据处理和报告交付串起来。

## 重要说明

- 本仓库提供的是学习路径、原创教程、视频脚本和实践项目，不替代当地法规、机型说明书、飞行许可或专业测绘资质要求。
- 实际飞行前，应以无人机制造商最新手册和所在地主管部门的最新规定为准。
- 测绘成果如果用于正式工程、权属、规划、司法或其他法定用途，应确认相应资质、坐标基准、精度要求和成果规范。

## 软件方向

建议先掌握一套主流程，再扩展：

- 航测处理：DJI Terra / WebODM / Agisoft Metashape（三选一作为主软件，另外两个用于理解差异）
- GIS：QGIS
- 数据格式：JPG/RAW、GeoTIFF、LAS/LAZ、OBJ/PLY、SHP/GeoPackage、KML/KMZ
- 后期：表格、图像标注、PDF报告

## 外部官方资料

- DJI Terra： https://www.dji.com/downloads/products/dji-terra
- QGIS 文档与培训手册： https://www.qgis.org/resources/hub/
- WebODM 文档： https://docs.webodm.org/
- Agisoft Metashape 手册： https://www.agisoft.com/pdf/metashape-pro_2_0_en.pdf

## 仓库目标

完成本课程后，你应该能够独立完成一个小型无人机测绘/巡检项目：

**需求理解 → 作业风险评估 → 航线设计 → 飞行采集 → 数据整理 → 三维/二维重建 → GIS分析 → 缺陷/目标标注 → 精度与质量检查 → 成果报告。**
