---
title: "EquationNode.ToMathML"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تحويل هذه المعادلة إلى تعبير MathML"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/tomathml/
---
## EquationNode.ToMathML method

تحويل هذه المعادلة إلى تعبير MathML.

```csharp
public string ToMathML()
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل معادلة - إضافة معامل العرض (300) ومعامل الارتفاع (100)
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // بناء معادلة بسيطة: (a+b)^2 = a^2 + 2ab + b^2
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
                // تحويل المعادلة إلى MathML
                string mathML = equation.ToMathML();

                // إخراج MathML إلى وحدة التحكم
                Console.WriteLine("MathML Output:");
                Console.WriteLine(mathML);

                // كتابة MathML إلى خلية
                worksheet.Cells["A1"].PutValue("MathML Representation:");
                worksheet.Cells["A2"].PutValue(mathML);
                // تم التغيير من worksheet.Cells.AutoFitColumns() إلى:
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting to MathML: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("EquationToMathMLDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


