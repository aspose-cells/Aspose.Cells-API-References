---
title: "ShapePath.WidthPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePath. يسترجع عرض هذا المسار بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

يحصل على عرض هذا المسار بوحدة البكسل.

```csharp
public int WidthPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // عرض قيمة WidthPixel الأولية
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // تعيين قيمة عرض جديدة
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // إضافة الشكل إلى ورقة العمل
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // احفظ المصنف
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


