---
title: "ShapePath.HeightPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePath. يسترجع ارتفاع هذا المسار بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

يحصل على ارتفاع هذا المسار بوحدة البكسل.

```csharp
public int HeightPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء مسار شكل جديد
                ShapePath shapePath = new ShapePath();

                // إنشاء مسار مستطيل بسيط
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // عرض قيمة HeightPixel الحالية
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // تعيين قيمة ارتفاع جديدة
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // إضافة الشكل إلى ورقة العمل
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // احفظ المصنف
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


