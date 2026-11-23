---
title: "EquationNode.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNode 属性。表示节点的类型"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/type/
---
## EquationNode.Type property

表示节点的类型。

```csharp
public override TextNodeType Type { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class EquationNodePropertyTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建方程形状
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationRoot = shape.GetEquationParagraph();

            // 创建不同类型的公式节点
            var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
            var textNode = equationRoot.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Text";

            // 显示不同节点的 Type 属性
            Console.WriteLine($"Root equation node type: {equationRoot.Type}");
            Console.WriteLine($"Fraction node type: {fractionNode.Type}");
            Console.WriteLine($"Text node type: {textNode.Type}");

            // 创建复杂的公式结构
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "Numerator";

            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "Denominator";

            // 检查子节点的类型
            Console.WriteLine($"Numerator node type: {numerator.Type}");
            Console.WriteLine($"Numerator text node type: {numeratorText.Type}");
            Console.WriteLine($"Denominator node type: {denominator.Type}");

            // 演示 Type 如何影响节点行为
            if (textNode.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("Text node is a TextRun type - can contain text content");
            }

            if (fractionNode.Type == TextNodeType.Equation)
            {
                Console.WriteLine("Fraction node is an Equation type - can contain child nodes");
            }

            // 保存结果
            workbook.Save("EquationNodePropertyTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


