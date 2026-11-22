---
title: "التعداد EquationFractionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Equations.EquationFractionType. يحدد هذا نمط عرض شريط الكسر"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

هذا يحدد نمط عرض شريط الكسر.

```csharp
public enum EquationFractionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Bar | `0` | يحدد هذا أن البسط فوق والمقام أسفل مفصولين بشريط في الوسط. |
| NoBar | `1` | يحدد هذا أن البسط فوق والمقام أسفل غير مفصولين بشريط في الوسط. |
| Linear | `2` | يحدد هذا أن البسط على اليسار والمقام على اليمين، مفصولين بـ '/' بينهما. |
| Skewed | `3` | يحدد هذا أن البسط في الأعلى اليسار والمقام في الأسفل اليمين، مفصولين بـ "/". |

### أمثلة

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
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على عقدة الرياضيات وأضف كسرًا
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
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
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


