---
layout: default
title: Apriori algorithm note
---
Apriori algorithm notes
====================

Apriori is a classic algorithm for frequent item set mining and association rule learning over transactional databases. It proceeds by identifying the frequent individual items in the database and extending them to larger and larger item sets as long as those item sets appear sufficiently often in the database. The frequent item sets determined by Apriori can be used to determine association rules which highlight general trends in the database: this has applications in domains such as market basket analysis.

一、Apriori算法简介：  Apriori算法是一种挖掘关联规则的频繁项集算法，其核心思想是通过候选集生成和情节的向下封闭检测两个阶段来挖掘频繁项集。 Apriori（先验的，推测的）算法应用广泛，可用于消费市场价格分析，猜测顾客的消费习惯；网络安全领域中的入侵检测技术；可用在用于高校管理中，根据挖掘规则可以有效地辅助学校管理部门有针对性的开展贫困助学工作；也可用在移动通信领域中，指导运营商的业务运营和辅助业务提供商的决策制定。

二、挖掘步骤：

1.依据支持度找出所有频繁项集（频度）

2.依据置信度产生关联规则（强度）

三、基本概念

对于A->B

①支持度：P(A ∩ B)，既有A又有B的概率

②置信度：

P(B|A)，在A发生的事件中同时发生B的概率 p(AB)/P(A)     例如购物篮分析：牛奶 ⇒ 面包

例子：[支持度：3%，置信度：40%]

支持度3%：意味着3%顾客同时购买牛奶和面包

置信度40%：意味着购买牛奶的顾客40%也购买面包

③如果事件A中包含k个元素，那么称这个事件A为k项集事件A满足最小支持度阈值的事件称为频繁k项集。

④同时满足最小支持度阈值和最小置信度阈值的规则称为强规则
dog's back.
![alt text](/jekyll_demo/images/apriori_products_example.jpg)
### 
### words
> support 支持度
> 
> confidence 置信度
>
> apriori 先验地，推测的，由原因推及结果的
>
> market basket analysis 购物篮分析
>
> association rule learning 关联规则发现
>
> frequent item set mining 频繁项集挖掘
>
>transactional databases 事务数据库
<p>{{page.date|date_to_string}}</p>
