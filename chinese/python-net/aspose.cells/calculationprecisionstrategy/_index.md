---
title: CalculationPrecisionStrategy枚举
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1820
url: /zh/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
## CalculationPrecisionStrategy枚举
枚举处理计算精度的策略。
由于 IEEE 754 Floating-Point Arithmetic 的精度问题，一些“看似简单”的公式可能无法计算出预期的结果。
如公式“=-0.45+0.43+0.02”，直接用'+'运算符计算操作数时，结果不为零。
一些特殊的策略可能会产生预期的结果。



CalculationPrecisionStrategy 类型公开了以下成员：

### 字段
|场地|描述|
| :- | :- |
| NONE |没有策略应用于计算。<br/>计算时直接用原来的double值作为操作数，直接返回结果即可。<br/>性能最有效，适用于大多数情况。|
| ROUND |计算结果按有效数字四舍五入。|
| DECIMAL |尽可能使用十进制作为操作数。<br/>性能效率最低。|



### 也可以看看
* 模块 [aspose.cells](..)
