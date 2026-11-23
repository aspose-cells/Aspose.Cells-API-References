---
title: "枚举 EquationNodeType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.EquationNodeType 枚举。方程节点类型。注意 1199 当前范围内只有一个节点，其枚举值为 1。它指定的节点用于存储数学文本。2100199 表示该节点是某些特殊函数节点的组成部分。3200 表示该节点具有一些特殊功能。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

方程节点类型。注意：(1)[1-99] 当前范围内只有一个节点，其枚举值为 1。它指定的节点用于存储数学文本。(2)[100-199] 表示该节点是某些特殊函数节点的组成部分。(3)[200-] 表示该节点具有一些特殊功能。

```csharp
public enum EquationNodeType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| UnKnow | `0` | 未知 |
| Text | `1` | 指定一个存储数学文本的节点 |
| Base | `100` | 指定一个 Base 组件 |
| Denominator | `101` | 指定一个 Denominator 组件 |
| Numerator | `102` | 指定一个 Numerator 组件 |
| FunctionName | `103` | 指定一个 FunctionName 组件 |
| Subscript | `104` | 指定一个 Subscript 组件 |
| Superscript | `105` | 指定一个 Superscript 组件 |
| Degree | `106` | 指定一个 Degree 组件 |
| MatrixRow | `107` | 指定一个 MatrixRow 组件。矩阵中的单行 |
| Limit | `108` | 表示 Lower-Limit 函数或 Upper-Limit 函数的子对象 |
| EquationParagraph | `200` | 指定一个数学段落（oMathPara）。 |
| MathematicalEquation | `201` | 指定一个方程或数学表达式（OMath）。 |
| FractionEquation | `202` | 指定分数方程 |
| FunctionEquation | `203` | 指定函数方程 |
| DelimiterEquation | `204` | 指定分隔符方程 |
| NaryEquation | `205` | 指定 n 元运算符方程 |
| RadicalEquation | `206` | 指定根式方程 |
| SuperscriptEquation | `207` | 指定上标方程 |
| SubscriptEquation | `208` | 指定下标方程 |
| SubSupEquation | `209` | 指定一个在操作数右侧带有上标和下标的方程。 |
| PreSubSupEquation | `210` | 指定一个在操作数左侧带有上标和下标的方程。 |
| AccentEquation | `211` | 指定重音方程 |
| BarEquation | `212` | 指定横线方程 |
| BorderBoxEquation | `213` | 指定边框盒子方程 |
| BoxEquation | `214` | 指定盒子方程 |
| GroupCharacterEquation | `215` | 指定组字符方程 |
| MatrixEquation | `216` | 指定矩阵方程， |
| LowerLimit | `217` | 指定下限函数 |
| UpperLimit | `218` | 指定上限函数 |
| Mathematical | `201` | 指定一个方程或数学表达式（OMath）。 |
| Fraction | `202` | 指定分数方程 |
| Function | `203` | 指定函数方程 |
| Delimiter | `204` | 指定分隔符方程 |
| Nary | `205` | 指定 n 元运算符方程 |
| Radical | `206` | 指定根式方程 |
| Sup | `207` | 指定上标方程 |
| Sub | `208` | 指定下标方程 |
| SubSup | `209` | 指定一个在操作数右侧带有上标和下标的方程。 |
| PreSubSup | `210` | 指定一个在操作数左侧带有上标和下标的方程。 |
| Accent | `211` | 指定重音方程 |
| Bar | `212` | 指定横线方程 |
| BorderBox | `213` | 指定边框盒子方程 |
| Box | `214` | 指定盒子方程 |
| GroupChr | `215` | 指定组字符方程 |
| Matrix | `216` | 指定矩阵方程， |
| ArrayEquation | `317` | 指定方程数组函数。该函数由一个或多个方程组成。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 在第一个工作表中添加公式
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 从方程中获取数学节点
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // 创建带有抑扬符字符的重音节点
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // 添加基节点和文本节点
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // 保存工作簿
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


