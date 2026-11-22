---
title: "EquationNode.ToLaTeX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. تحويل هذه المعادلة إلى تعبير LaTeX"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

تحويل هذه المعادلة إلى تعبير LaTeX.

```csharp
public string ToLaTeX()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToLaTeXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاحتواء المعادلة
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // الحصول على عقدة المعادلة
            var equationNode = shape.GetEquationParagraph();

            // إنشاء معادلة كسر بسيطة
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // استدعاء طريقة ToLaTeX
                string latexExpression = equationNode.ToLaTeX();
                
                // اعرض النتيجة
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // إضافة ناتج LaTeX إلى خلية
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


