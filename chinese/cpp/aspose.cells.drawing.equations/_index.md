---
title: "Aspose::Cells::Drawing::Equations 命名空间"
linktitle: "Aspose::Cells::Drawing::Equations"
second_title: "Aspose.Cells for C++ API 参考"
description: "如何在 C++ 中使用 Aspose::Cells::Drawing::Equations 命名空间。"
type: docs
weight: 700
url: /zh/cpp/aspose.cells.drawing.equations/
---



## 类

| 类 | 描述 |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | 此类指定一个重音等式，由基组件和组合变音符组成。 |
| [ArrayEquationNode](./arrayequationnode/) | 指定 Equation-Array 函数，一个由一个或多个等式组成的对象。 |
| [BarEquationNode](./barequationnode/) | 此类指定 bar 等式，由基参数和上划线或下划线组成。 |
| [BorderBoxEquationNode](./borderboxequationnode/) | 此类指定 [边框](../aspose.cells/border/) Box 函数，由围绕等式绘制的边框组成。 |
| [BoxEquationNode](./boxequationnode/) | 此类指定 box 函数，用于对等式的组件进行分组。 |
| [DelimiterEquationNode](./delimiterequationnode/) | 此类指定分隔符等式，由左、右分隔符（例如圆括号、花括号、方括号和竖线）以及其中包含的组件组成。分隔符可以包含多个组件，每个组件之间使用指定的分隔字符。 |
| [EquationComponentNode](./equationcomponentnode/) | 此类指定等式或数学表达式的组件。不同类型的组件组合成不同的等式。例如，分数由两个部分组成，即分子组件和分母组件。有关更多组件类型，请参阅 “EquationNodeType”。 |
| [EquationNode](./equationnode/) | 用于派生其他等式节点的抽象类。 |
| [EquationNodeParagraph](./equationnodeparagraph/) | 此类指定包含一个或多个 MathEquationNode（OMath）元素的数学段落。 |
| [FractionEquationNode](./fractionequationnode/) | 此类指定分数等式，由分子和分母通过分数线分隔。分数线可以是水平或对角线，取决于分数属性。分数等式还用于表示堆叠函数，即将一个元素放在另一个元素之上且不使用分数线。 |
| [FunctionEquationNode](./functionequationnode/) | 此类指定 Function-Apply 等式，由函数名和被作用的参数组成。名称和参数组件的类型分别为 '[EquationNodeType.FunctionName](./equationnodetype/)' 和 '[EquationNodeType.Base](./equationnodetype/)'。 |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | 此类指定 Group-Character 函数，由绘制在文本上方或下方的字符组成，通常用于视觉上对项目进行分组。 |
| [LimLowUppEquationNode](./limlowuppequationnode/) | 此类指定极限函数。 |
| [MathematicalEquationNode](./mathematicalequationnode/) | 此类指定等式或数学表达式。所有等式或数学表达式的数学文本均由此类包含。 |
| [MatrixEquationNode](./matrixequationnode/) | 此类指定矩阵等式，由一个或多个元素按一个或多个行和一个或多个列排列组成。 |
| [NaryEquationNode](./naryequationnode/) | 此类指定 n 元运算符等式，由 n 元运算符、基（或操作数）以及可选的上界和下界组成。 |
| [RadicalEquationNode](./radicalequationnode/) | 此类指定根式等式，由可选的次数 deg([EquationNodeType.Degree](./equationnodetype/)) 和基组成。 |
| [SubSupEquationNode](./subsupequationnode/) | 此类指定可以选择性地为上标或下标的等式。该等式主要有四种形式：上标、下标、上标和下标位于基的左侧、上标和下标位于基的右侧。 |
| [TextRunEquationNode](./textrunequationnode/) | 等式节点中的此类用于存储等式的实际内容（数学文本序列）。通常每个字符对应一个节点对象。 |
| [UnknowEquationNode](./unknowequationnode/) | 未知类型的等式节点类。 |
## Enums

| 枚举 | 描述 |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | 指定子对象在其父对象中的位置。 |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | 组合字符的类型。 |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | 这指定了分隔符对象中分隔符的形状。 |
| [EquationFractionType](./equationfractiontype/) | 这指定了分数线的显示样式。 |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | 这指定了文档中公式的默认水平对齐方式。 |
| [EquationLimitLocationType](./equationlimitlocationtype/) | 指定运算符的极限位置。 |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | 数学运算符类型。 |
| [EquationNodeType](./equationnodetype/) | 方程节点类型。注意：(1)[1-99] 当前范围内只有一个节点，其枚举值为 1。它指定的节点用于存储数学文本。(2)[100-199] 表示该节点是某些特殊函数节点的组成部分。(3)[200-] 表示该节点具有一些特殊功能。 |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | 这指定了文档中公式的默认垂直对齐方式。 |
