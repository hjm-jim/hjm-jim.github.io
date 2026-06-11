---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

---
---
name: 胡景明
header:
  - text: <span class="iconify" data-icon="tabler:phone"></span> 181-6401-2616
    newLine: true
  - text: <span class="iconify" data-icon="tabler:mail"></span> jimmyh2020@163.com
    link: mailto:jimmyh2020@163.com
  - text: <span class="iconify" data-icon="tabler:brand-github"></span> 个人作品页
    link: https://word.tyger.wszgdhz.com/units
---

<!-- Important: Replace all template content, especially contact details, with your own information. -->

<!-- Important: When updating your email address, remember to change both the "text" (visible text) and the "link" (underlying hyperlink) fields. -->


## 教育经历

**武汉大学**

计算机科学与技术    硕士
  ~ 2024.9 - 2027.6

**武汉大学**

信息安全          本科
  ~ 2020.9 - 2024.6


## 实习项目经历

**Agent开发工程师**
  ~ 武汉长江水利委员会
  ~ 2025.3 – 2025.7

- **背景与痛点**：水利领域法规/规范结构复杂，传统人工提取单份文件耗时约 **40分钟**，易遗漏重要条款；巡河人员现场急需快速获得问答获取规范依据，提出详细合规的整改意见。

- **职责与方案**：访谈 **10+** 水利院一线成员，抽象出业务本质是 **知识找人** 而非人找知识，且要求识图理解（施工场布现场读图，补充一线成员的描述）与法律遵循句句落实（每一条回答必须可追溯到规范原文）。最终敲定 AI工作流+规则引擎+检索增强生成（RAG） 的协同办公级方案。

- **细分模块落地**：

  🔴知识理解：对表格、嵌套条款、引用关系建立专门化规则引擎，转化为结构化知识节点统一入库。对于无结构文本，采用段落滑动窗口分块+打标入库。

  🔴法律遵循：每一条模型输出格式强制关联原文位置 + 引用链路，做到 “句句有依据”。

  🔴向量检索：采用标签索引作为辅助检索向量，部署QWEN3-4B embedding模型+Milvus向量数据库。

  🔴优雅着陆：轻量纠错模型+人工反馈作为后处理层，不符合规范表述的生成内容，后台作为badcase优化模型，驱动迭代。

- **产出成果**：系统形成一项专利；相比于人工录入，入库效率提效5倍以上；召回准确率提升约5%；实现了领域专门知识从死板文本到问即所得，知识找人的闭环。

**G端网络安全流量监控项目**
  ~ 武汉大学珞珈之戍实验室
  ~ 2025.4 - 2026.4

- **职责与方案**：
辅助**G端数字化**单位用户监控企业内网到外网的流量。期望对窃密、泄密行为做到**早感知，快定位，准取证**。作为项目技术负责人，和客户深度交流，敲定技术细节和生产环境实施方案。

  🔴整体方案：部署在网关作为web应用层IPS的一部分，以TCP/IP中间人形式分析端到端网络流量。

  🔴实现方案：为避免明显的开源工具流量指纹，重新实现TLS各协议版本、密码套件，包含密钥协商、哈希函数、数字签名等密码算法。截获的流量在**内网数据库**存储留档，G端管理人员通过域名+时间+关键词正则匹配窃密流量信息，精确定位窃密人员。

  🔴实施方案：采用docker容器化打包、部署整个IPS流量处理环境，使内网受限用户**开箱即用**；在部署初期查看服务状态，工作日志等信息，确保容器**高可用**性；结合wireshark工具进行网络抓包，对“网太慢”这种大类问题进行**归因、测试**，定位bug或高负载瓶颈。

- **产出成果**：容器健康状态下单条数据包的处理时延低于1ms。团队协助3家G端单位落地系统。

**B端ERP产品经理**
  ~ 无锡帆软软件有限公司
  ~ 2025.12 - 2026.2
- **职责与方案**：熟悉B端客户使用表单类零代码应用的主流场景，协助调研 FineBI / 九数云 / 简道云 RBAC权限体系细节，产出竞品分析报告和权限坑点文档。
- **产出成果**：提炼「僵尸权限」等核心痛点。独立编写权限体系兼容升级方案，加入产品团队任务蓝图。

## 近期荣誉

**揭榜挂帅"挑战杯" · 武汉大学团队**  <span style="float:right">2025.7 – 2025.9</span>
- 针对工业互联网设计数字孪生模型，主持 10+ 次组会，比赛获 **全国二等奖**。


## 技能

- **计算机通用能力:**  <span class="iconify" data-icon="vscode-icons:file-type-python"></span> Python、<span class="iconify" data-icon="vscode-icons:file-type-sql"></span>sql熟练，计算机网络、操作系统原理扎实，有全栈开发经验。

- **AI能力:** 熟练使用claude code，擅长搭建dify、coze等提效工具，擅长本地部署AI模型。

- **外语:** 英语（六级604，工作语言） ，法语（B1）
