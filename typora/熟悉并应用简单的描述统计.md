[TOC]



## 熟悉并应用简单的描述统计

### 一. 什么是统计学

**统计学**是在资料分析的基础上，研究测定、收集、整理、归纳和分析反映数据资料，以便给出正确消息的科学。这一门学科自17世纪中叶产生并逐步发展起来，它广泛地应用在各门[学科](https://zh.wikipedia.org/wiki/學科列表)，从[自然科学](https://zh.wikipedia.org/wiki/自然科学)、[社会科学](https://zh.wikipedia.org/wiki/社會科學)到[人文学科](https://zh.wikipedia.org/wiki/人文学科)，甚至被用于[工商业](https://zh.wikipedia.org/wiki/工商業)及[政府](https://zh.wikipedia.org/wiki/政府)的情报决策。随着[大数据](https://zh.wikipedia.org/wiki/大数据)时代来临，统计的面貌也逐渐改变，与信息、计算等领域密切结合，是[数据科学](https://zh.wikipedia.org/wiki/数据科学)中的重要主轴之一。

数据分析所用的方法可分为**描述统计方法**和**推断统计方法**。描述统计研究的是数据收集、处理、汇总、图表描述、概括与分析等统计方法。推断统计是研究如何利用样本数据来推断总体特征的统计方法。



### 二. 统计指标



#### **平均数**

为[集中趋势](https://zh.wikipedia.org/wiki/集中趋势)的最常用测度值，目的是确定一组数据的均衡点。

- 平均数容易受到异常数据的影响。

#### **四分位数**

即把所有数值由小到大排列并分成四等份，处于三个分割点位置的数值就是四分位数。

#### **Tukey's test**

 a single-step [multiple comparison](https://en.wikipedia.org/wiki/Multiple_comparison) procedure and [statistical test](https://en.wikipedia.org/wiki/Statistical_test). It can be used to find means that are [significantly](https://en.wikipedia.org/wiki/Statistical_significance) different from each other.

1. 最小估计值：
   $$
   Q1 - k(Q3 - Q1)
   $$

2. 最大估计值：
   $$
   Q3 + k(Q3 - Q1)
   $$

3. k = 1.5 时，中度异常

4. k = 3 时，极度异常



#### **标准差**

在[概率](https://zh.wikipedia.org/wiki/概率)[统计](https://zh.wikipedia.org/wiki/統計)中最常使用作为[测量](https://zh.wikipedia.org/wiki/測量)一组数值的[离散程度](https://zh.wikipedia.org/wiki/离散程度)之用。标准差定义：为[方差](https://zh.wikipedia.org/wiki/方差)开[算术平方根](https://zh.wikipedia.org/wiki/算术平方根)，反映组内个体间的离散程度；标准差与[期望值](https://zh.wikipedia.org/wiki/期望值)之比为标准离差率。

#### **标准分**

距平均值多少个标准差，一定程度上可以比较不同类别数据中个体的的离散度。

#### **变异系数**

是[概率分布](https://zh.wikipedia.org/wiki/概率分布)离散程度的一个[归一化](https://zh.wikipedia.org/wiki/歸一化)量度，其定义为[标准差](https://zh.wikipedia.org/wiki/标准差)与平均值之比，可以用来比较不同数据集整体的离散程度。

## 三.数据集的信息

#### 1.购买商品信息

| 字段      | 含义         |
| --------- | ------------ |
| user_id   | 用户ID       |
| item_id   | 商品id       |
| cat_id    | 商品二级分类 |
| cat1      | 商品一级分类 |
| property  | 商品的属性值 |
| buy_mount | 购买数量     |
| day       | 购买日期     |



#### 2.婴儿信息

| 字段名称 | 含义                   |
| -------- | ---------------------- |
| user_id  | 用户ID                 |
| birthday | 出生日期(eg. 20130423) |
| gender   | 性别 0:女性 1:男性     |

### 四.能够分析的业务问题

#### 业务问题

1. 哪个月商品销量最高
2. 能否得知某个年龄段或者性别对产品偏好的不同
3. 类似2，能否得知每个用户的购买偏好
4. 哪个商品的重复购买率最高

#### 如何解决这些问题

1. 通过数据集中的购买数量与购买日期中的月份作折线图/柱状体得出
2. 通过数据集中的性别/出生日期时间段对每个二级分类商品作饼图得出
3. 计算用户购买的商品从属的一级与二级分类总数，制定简单算法计算其偏好
4. 计算每个商品在每个用户的重复购买次数（不同时间）







