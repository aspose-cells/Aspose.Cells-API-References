---
title: "FractionEquationNode.FractionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FractionEquationNode. تحدد نوع الكسر، القيمة الافتراضية هي Bar"
type: docs
url: /ar/net/aspose.cells.drawing.equations/fractionequationnode/fractiontype/
---
## FractionEquationNode.FractionType property

هذا يحدد نوع الكسر؛ القيمة الافتراضية هي 'Bar'.

```csharp
public EquationFractionType FractionType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FractionEquationNodePropertyFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة الرياضيات
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إنشاء عقدة كسر
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // إضافة البسط
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // إضافة المقام
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // حفظ والتحقق
            string outputPath = "FractionEquationDemo.xlsx";
            workbook.Save(outputPath);

            // أعد التحميل للتحقق
            Workbook verifyWorkbook = new Workbook(outputPath);
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            FractionEquationNode verifyFraction = (FractionEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Fraction Type: " + verifyFraction.FractionType);
            Console.WriteLine("Numerator: " + ((TextRunEquationNode)verifyFraction.GetChild(0).GetChild(0)).Text);
            Console.WriteLine("Denominator: " + ((TextRunEquationNode)verifyFraction.GetChild(1).GetChild(0)).Text);
        }
    }
}
```

### انظر أيضًا

* enum [EquationFractionType](../../equationfractiontype/)
* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


