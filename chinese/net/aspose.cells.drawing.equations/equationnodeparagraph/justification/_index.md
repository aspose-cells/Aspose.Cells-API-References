---
title: "EquationNodeParagraph.Justification"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNodeParagraph 属性。此属性指定同一段落中相邻方程组成的数学段落的对齐方式。数学段落可以是左对齐、右对齐、居中或整体居中。默认情况下，数学段落是整体居中。这意味着方程可以相互对齐，但整个方程组整体居中。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

这指定了数学段落的对齐方式（同一段落内相邻方程的系列）。数学段落可以是左对齐、右对齐、居中或整体居中。默认情况下，数学段落是整体居中。这意味着方程之间可以相互对齐，但整个方程组整体居中。

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个用于容纳方程的形状
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Get the equation paragraph
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // 显示当前对齐值
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // 设置不同的对齐值并观察效果
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // 保存工作簿
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


