<p align="center"><a href="https://dataease.io"><img src="https://dataease.oss-cn-hangzhou.aliyuncs.com/img/dataease-logo.png" alt="DataEase" width="300" /></a></p>
<h3 align="center">人人可用的开源 BI 工具</h3>
<p align="center">
  <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/github/license/dataease/dataease?color=%231890FF" alt="License: GPL v3"></a>
  <a href="https://app.codacy.com/gh/dataease/dataease?utm_source=github.com&utm_medium=referral&utm_content=dataease/dataease&utm_campaign=Badge_Grade_Dashboard"><img src="https://app.codacy.com/project/badge/Grade/da67574fd82b473992781d1386b937ef" alt="Codacy"></a>
  <a href="https://github.com/dataease/dataease"><img src="https://img.shields.io/github/stars/dataease/dataease?color=%231890FF&style=flat-square" alt="GitHub Stars"></a>
  <a href="https://gitee.com/fit2cloud-feizhiyun/DataEase"><img src="https://gitee.com/fit2cloud-feizhiyun/DataEase/badge/star.svg?theme=gvp" alt="Gitee Stars"></a><br>
  [<a href="/README.md">中文(简体)</a>] | [<a href="/docs/README.en.md">English</a>] | [<a href="/docs/README.ja.md">日本語</a>]
</p>

------------------------------

## 什么是 DataEase？

DataEase 是开源的 BI 工具，帮助用户快速分析数据并洞察业务趋势，从而实现业务的改进与优化。DataEase 支持丰富的数据源连接，能够通过拖拉拽方式快速制作图表，并可以方便的与他人分享。

**DataEase 的优势：**

-   开源开放：零门槛，线上快速获取和安装，按月迭代；
-   简单易用：极易上手，通过鼠标点击和拖拽即可完成分析；
-   全场景支持：多平台安装和多样化嵌入支持；
-   安全分享：支持多种数据分享方式，确保数据安全。

**DataEase 支持的数据源：**

-   OLTP 数据库： MySQL、Oracle、SQL Server、PostgreSQL、MariaDB、Db2、TiDB、MongoDB-BI 等；
-   OLAP 数据库： ClickHouse、Apache Doris、Apache Impala、StarRocks 等；
-   数据仓库/数据湖： Amazon RedShift 等；
-   数据文件： Excel、CSV 等；
-   API 数据源。

如果您需要向团队介绍 DataEase，可以使用这个 [官方 PPT 材料](https://fit2cloud.com/dataease/download/introduce-dataease_202411.pdf)。

## 快速开始

**桌面版：**

你可以在 PC 上安装 DataEasae 桌面版，下载地址为：https://dataease.cn/

**服务器版：**

```
# 准备一台 2 核 4G 以上的 Linux 服务器，并以 root 用户运行以下一键安装脚本：

curl -sSL https://dataease.oss-cn-hangzhou.aliyuncs.com/quick_start_v2.sh | bash

# 用户名: admin
# 密码: DataEase@123456
```

你也可以通过 [1Panel 应用商店](https://dataease.io/docs/v2/installation/1panel_installation/) 快速部署 DataEase。如果是用于生产环境，推荐使用 [离线安装包方式](https://dataease.io/docs/v2/installation/offline_INSTL_and_UPG/) 进行安装部署。

如你有更多问题，可以查看在线文档，或者通过论坛与我们交流。

-   [在线文档](https://dataease.io/docs/)
-   [社区论坛](https://bbs.fit2cloud.com/c/de/6)
-   [案例研究](/docs/use-cases.md)

## UI 展示

<table style="border-collapse: collapse; border: 1px solid black;">
  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/8dbed4e1-39f0-4392-aa8c-d1fd83ba42eb" alt="DataEase 工作台"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/7c54cb07-51ef-4bb6-a931-8a95c64c7e11" alt="DataEase 仪表板"   /></td>
  </tr>

  <tr>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/ffa79361-a7b3-4486-b14a-f3fd3a28f01a" alt="DataEase 数据源"   /></td>
    <td style="padding: 5px;background-color:#fff;"><img src= "https://github.com/dataease/dataease/assets/41712985/bb28f4e4-636e-4ab0-85c5-1dfbd7a5397e" alt="DataEase 模板中心"   /></td>
  </tr>
</table>

## 技术栈

-   前端：[Vue.js](https://vuejs.org/)、[Element](https://element.eleme.cn/)
-   图库：[AntV](https://antv.vision/zh)
-   后端：[Spring Boot](https://spring.io/projects/spring-boot)
-   数据库：[MySQL](https://www.mysql.com/)
-   数据处理：[Apache Calcite](https://github.com/apache/calcite/)、[Apache SeaTunnel](https://github.com/apache/seatunnel)
-   基础设施：[Docker](https://www.docker.com/)

这是一个现代技术栈的组合，非常适合开发企业级或数据驱动型的应用程序。以下是对各技术的简要说明以及它们如何协同工作：

---

### **前端：Vue.js、Element**
- **Vue.js**: 一个流行的前端框架，提供高效的组件化开发，适用于响应式和交互式的用户界面。
- **Element**: 基于 Vue 的 UI 组件库，包含丰富的组件（如表单、表格、对话框等），适合快速构建美观、统一的前端界面。


### **图库：AntV**
- **AntV**: 一个强大的数据可视化库，支持多种图表（折线图、柱状图、关系图等）和交互设计，非常适合构建数据分析应用。

### **后端：Spring Boot**
- **Spring Boot**: 一个轻量级的 Java 框架，便于快速构建生产级的后端应用，支持多种数据库、RESTful 接口以及微服务架构。


### **数据库：MySQL**
- **MySQL**: 一个开源关系型数据库，适用于存储结构化数据，支持高效的查询操作和事务管理。
- 可与 Spring Boot 无缝集成，通过 JPA 或 MyBatis 实现数据的持久化。


### **数据处理：Apache Calcite、Apache SeaTunnel**
- **Apache Calcite**: 一个动态数据管理框架，支持 SQL 查询的解析、优化和执行，可以作为数据处理的核心组件。
- **Apache SeaTunnel**: 一个数据集成工具，支持批处理和流处理，适合构建 ETL（提取、转换、加载）管道。

### **基础设施：Docker**
- **Docker**: 一个容器化平台，可以轻松实现应用的打包、分发和部署。适合构建微服务架构和支持快速扩展。

---

### **协作方式**
1. **数据流**：
   - 用户通过 Vue.js 前端与系统交互。
   - Element 提供友好的用户界面。
   - 用户行为或数据输入通过 API 请求发送到 Spring Boot 后端。
   - Spring Boot 使用 MySQL 存储或查询数据，并通过 AntV 在前端展示分析结果。

2. **数据处理**：
   - Apache SeaTunnel 负责数据的采集和预处理。
   - Apache Calcite 负责动态执行复杂的 SQL 查询，提升数据处理效率。

3. **部署**：
   - Docker 用于将前端、后端、数据库和数据处理工具封装成独立的容器，方便部署到云平台。

这种组合既现代又灵活，适合大多数企业级应用开发需求。如果有特定的场景或项目需求，可以进一步定制和优化技术选型。

## 飞致云的其他明星项目

- [1Panel](https://github.com/1panel-dev/1panel/) - 现代化、开源的 Linux 服务器运维管理面板
- [MaxKB](https://github.com/1panel-dev/MaxKB/) - 基于 LLM 大语言模型的开源知识库问答系统
- [JumpServer](https://github.com/jumpserver/jumpserver/) - 广受欢迎的开源堡垒机
- [Halo](https://github.com/halo-dev/halo/) - 强大易用的开源建站工具
- [MeterSphere](https://github.com/metersphere/metersphere/) - 新一代的开源持续测试工具

## License

Copyright (c) 2014-2024 [FIT2CLOUD 飞致云](https://fit2cloud.com/), All rights reserved.

Licensed under The GNU General Public License version 3 (GPLv3)  (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

<https://www.gnu.org/licenses/gpl-3.0.html>

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
