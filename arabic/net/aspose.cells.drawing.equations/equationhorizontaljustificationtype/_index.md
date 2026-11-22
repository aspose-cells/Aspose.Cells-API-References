---
title: "تعداد EquationHorizontalJustificationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType تعداد. يحدد هذا المحاذاة الأفقية الافتراضية للمعادلات في المستند"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

هذا يحدد المحاذاة الأفقية الافتراضية للمعادلات في المستند.

```csharp
public enum EquationHorizontalJustificationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Center | `0` | متمركز |
| CenterGroup | `1` | متمركز كمجموعة |
| Left | `2` | محاذاة إلى اليسار |
| Right | `3` | محاذاة إلى اليمين |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف شكل معادلة إلى ورقة العمل
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // احصل على فقرة المعادلة
                EquationNodeParagraph equationNode = (EquationNodeParagraph)textBox.GetEquationParagraph();

                // عرض أنواع مختلفة من المحاذاة الأفقية
                equationNode.Justification = EquationHorizontalJustificationType.Center;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Left;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Right;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                // احفظ المصنف
                workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationHorizontalJustificationType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


