---
title: "تعداد ShapeTextVerticalAlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.ShapeTextVerticalAlignmentType enum. يتطابق مع Format Shape  Text Options  Text Box  Vertical Alignment في Excel"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextverticalalignmenttype/
---
## ShapeTextVerticalAlignmentType enumeration

يتطابق مع "Format Shape - Text Options - Text Box - Vertical Alignment" في Excel.

```csharp
public enum ShapeTextVerticalAlignmentType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Top | `0` |  |
| Middle | `1` |  |
| Bottom | `2` |  |
| TopCentered | `3` |  |
| MiddleCentered | `4` |  |
| BottomCentered | `5` |  |
| Left | `6` |  |
| Center | `7` |  |
| Right | `8` |  |
| LeftMiddle | `9` |  |
| CenterMiddle | `10` |  |
| RightMiddle | `11` |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassShapeTextVerticalAlignmentTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة مربع نص إلى ورقة العمل
                var textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 300);
                textBox.Text = "Sample text for vertical alignment demonstration";

                // تعيين محاذاة النص العمودية إلى الوسط
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;

                // عرض المحاذاة العمودية الحالية
                Console.WriteLine("Current vertical alignment: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // تغيير إلى محاذاة أعلى
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
                Console.WriteLine("Changed to: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // احفظ المصنف
                workbook.Save("ShapeTextVerticalAlignmentTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapeTextVerticalAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


