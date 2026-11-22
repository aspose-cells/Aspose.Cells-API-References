---
title: "FontSettingCollection.TextAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSettingCollection. تمثل إعداد محاذاة نص الجسم"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/textalignment/
---
## FontSettingCollection.TextAlignment property

تمثل إعداد محاذاة جسم النص.

```csharp
public ShapeTextAlignment TextAlignment { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            shape.Text = "Sample Text";

            // الوصول إلى خصائص TextAlignment وتعديلها
            var textAlignment = shape.TextBody.TextAlignment;
            
            Console.WriteLine("Default Margins (Points):");
            Console.WriteLine($"AutoMargin: {textAlignment.IsAutoMargin}");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");

            // تعديل الهوامش
            textAlignment.TopMarginPt = 36;
            textAlignment.BottomMarginPt = 36;
            textAlignment.LeftMarginPt = 18;
            textAlignment.RightMarginPt = 18;

            // احفظ المصنف
            workbook.Save("TextAlignmentDemo.xlsx");

            Console.WriteLine("\nModified Margins (Points):");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


