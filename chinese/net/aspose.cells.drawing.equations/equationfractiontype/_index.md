---
title: "枚举 EquationFractionType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Equations.EquationFractionType 枚举。此指定分数线的显示样式"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

此项指定分数线的显示样式。

```csharp
public enum EquationFractionType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Bar | `0` | 此指定分子在上方，分母在下方，中间用一条横线分隔。 |
| NoBar | `1` | 此指定分子在上方，分母在下方，中间不使用横线分隔。 |
| Linear | `2` | 此指定分子在左侧，分母在右侧，两者之间用 '/' 分隔。 |
| Skewed | `3` | 此指定分子在左上，分母在右下，两者之间用 \"/\" 分隔。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加公式形状
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // 获取数学节点并添加分数
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // 添加分子
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // 添加分母
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // 保存并验证
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


