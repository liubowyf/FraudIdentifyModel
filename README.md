# 涉诈预警发现模型1.0版本

## 背景

在当今数字化时代，随着互联网技术的迅猛发展，网络空间已经成为人们日常生活中不可或缺的一部分。然而，网络环境的开放性和匿名性也为不法分子提供了实施诈骗的机会，导致电信网络诈骗案件频发，对公众财产安全和社会稳定造成了严重影响。

面对日益复杂的诈骗手段，如传统的冒充身份、虚假购物以及新兴的“杀猪盘”、贷款诈骗、刷单返利等，我们迫切需要构建一个高效且智能的涉诈预警发现模型。该项目通过整合大数据分析、人工智能算法及机器学习等先进技术，旨在建立一套能够实时监控并精准预警的反诈骗系统。该系统将利用公安机关提供的涉案号码及相关案件数据进行深度挖掘与智能分析，识别诈骗模式与风险特征，并针对高发类型的诈骗案件提供即时预警服务。

本项目的核心目标是减少诈骗案件的发生率，保护人民的财产安全，同时提高社会公众的防诈骗意识和自我防护能力。系统能够自动识别潜在受害者，并在诈骗行为发生之前，通过短信、电话等多种渠道向用户发送个性化预警信息，指导其采取预防措施。此外，系统还能联动警方快速响应，有效遏制诈骗案件的蔓延趋势。

## 现状

截至2024年中，第一版涉诈网站预警模型已经开发完成并投入使用。此模型每天处理8千万到1亿条PDNS网站域名访问记录，平均每日识别出约4000个涉诈网站。根据公安部公告的14大网络涉诈分类标准，这些网站被进一步分类，包括但不限于：冒充电商物流客服类、冒充公检法及政府机关类、刷单返利类等。

## 特性

该软件的核心功能由三重降噪与发现机制加上一项行业特殊手段构成（简称3+1模型）：

### 一重降噪
基于PDNS海量数据集的数据降噪过程，采用白名单机制和域名特征分析算法，筛选出可能涉及诈骗活动的高风险数据，为进一步分析奠定基础。

### 二重发现
模拟用户行为访问疑似涉诈网站，收集并保存相关信息。使用预先归纳整理的涉诈标签（例如特征文本和依赖组件），结合复杂的内容匹配权重算法，对达到特定阈值的网站进行涉诈判定。

### 三重拓线
深入分析涉诈网站的相关联网址，揭示隐藏的关联关系，扩大预警范围。

### 行业特殊手段
这部分内容暂不公开讨论，它涉及获取诈骗方和受害人的详细信息。后续我们将专注于涉诈发现能力的提升和技术细节。

![示意图](https://github.com/user-attachments/assets/a2140942-6e37-4cf2-b931-a08f338b5d6e)

## 优点

1. 支持大规模网站分析，具备极高的处理效率。
2. 可以从特定或一类涉诈网站中提取大量特征标签，有助于后续同类网站的识别工作。

## 缺点

1. 尽管已收集了超过1700个特征标签，但随着新型涉诈网站的不断涌现，现有特征的有效性正在减弱。加之许多网站采用了反爬虫策略，增加了识别难度。
2. 不同涉诈分类所使用的特征匹配逻辑各异，这使得模型在适应不同类型的诈骗时面临挑战，并需随时间调整算法以应对诈骗手法的变化。
3. 特征标签的人工分析和归纳占据了较大比重，为了防止误判，还需投入大量人力进行前期验证工作。

## 局限

鉴于上述问题，当前模型在跟上犯罪分子技术升级步伐方面存在局限。特别是对于新出现的诈骗标签特征召回率较低，特征收集已达瓶颈。因此，急需探索新的技术和方法来升级涉诈预警发现模型，即进入2.0版本的研发阶段，涵盖理论研究、技术选型、架构设计及工程实现等多个层面。

# 涉诈预警发现模型2.0版本




