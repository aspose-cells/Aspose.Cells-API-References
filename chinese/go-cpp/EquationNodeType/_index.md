---
title: "EquationNodeType 枚举"
linktitle: "EquationNodeType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "EquationNodeType 枚举。封装了在 Go 中表示 equationnodetype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/equationnodetype/
---

## EquationNodeType Enum

方程节点类型。注意：(1)[1-99] 当前范围内只有一个节点，其枚举值为 1。它指定的节点用于存储数学文本。(2)[100-199] 表示该节点是某些特殊函数节点的组成部分。(3)[200-] 表示该节点具有一些特殊功能。

```go

type EquationNodeType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [UnKnow](./unknow/) | 未知 |
| [Text](./text/) | 指定存储数学文本的节点 |
| [Base](./base/) | 指定基础组件 |
| [Denominator](./denominator/) | 指定分母组件 |
| [Numerator](./numerator/) | 指定分子组件 |
| [FunctionName](./functionname/) | 指定函数名组件 |
| [Subscript](./subscript/) | 指定下标组件 |
| [Superscript](./superscript/) | 指定上标组件 |
| [Degree](./degree/) | 指定指数组件 |
| [MatrixRow](./matrixrow/) | 指定 MatrixRow 组件。矩阵中的单行 |
| [Limit](./limit/) | 表示下限函数或上限函数的子对象 |
| [EquationParagraph](./equationparagraph/) | 指定数学段落（oMathPara）。 |
| [LowerLimit](./lowerlimit/) | 指定下限函数 |
| [UpperLimit](./upperlimit/) | 指定上限函数 |
| [Mathematical](./mathematical/) | 指定方程或数学表达式（OMath）。 |
| [Fraction](./fraction/) | 指定分数方程 |
| [Function](./function/) | 指定函数方程 |
| [Delimiter](./delimiter/) | 指定分隔符方程 |
| [Nary](./nary/) | 指定 n 元运算符方程 |
| [Radical](./radical/) | 指定根式方程 |
| [Sup](./sup/) | 指定上标方程 |
| [Sub](./sub/) | 指定下标方程 |
| [SubSup](./subsup/) | 指定一个上标和下标位于操作数右侧的方程。 |
| [PreSubSup](./presubsup/) | 指定一个上标和下标位于操作数左侧的方程。 |
| [Accent](./accent/) | 指定重音方程 |
| [Bar](./bar/) | 指定条形方程 |
| [BorderBox](./borderbox/) | 指定边框盒子方程 |
| [Box](./box/) | 指定盒子方程 |
| [GroupChr](./groupchr/) | 指定组字符方程 |
| [Matrix](./matrix/) | 指定矩阵方程， |
| [ArrayEquation](./arrayequation/) | 指定方程数组函数。该函数由一个或多个方程组成。 |
