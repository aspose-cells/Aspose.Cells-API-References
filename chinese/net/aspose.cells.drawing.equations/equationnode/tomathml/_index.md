---
title: "EquationNode.ToMathML"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationNode 方法。将此方程转换为 MathML 表达式"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationnode/tomathml/
---
## EquationNode.ToMathML method

将此等式转换为 MathML 表达式。

```csharp
public string ToMathML()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToMathMLDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个方程形状 - 添加宽度参数 (300) 和高度参数 (100)
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // 构建一个简单方程: (a+b)^2 = a^2 + 2ab + b^2
            var equationNode = equation.AddChild(EquationNodeType.Text);
            var textNode = equationNode as TextRunEquationNode;
            textNode.Text = "(";

            var variableA = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableA.Text = "a";

            var plus = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            plus.Text = "+";

            var variableB = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableB.Text = "b";

            var closeParen = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            closeParen.Text = ")";

            var superscript = equation.AddChild(EquationNodeType.Superscript);
            var baseNode = superscript.AddChild(EquationNodeType.Base);
            var baseText = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            baseText.Text = "2";

            try
            {
                // 将方程转换为 MathML
                string mathML = equation.ToMathML();

                // 将 MathML 输出到控制台
                Console.WriteLine("MathML Output:");
                Console.WriteLine(mathML);

                // 将 MathML 写入单元格
                worksheet.Cells["A1"].PutValue("MathML Representation:");
                worksheet.Cells["A2"].PutValue(mathML);
                // 已从 worksheet.Cells.AutoFitColumns() 更改为：
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting to MathML: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("EquationToMathMLDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


