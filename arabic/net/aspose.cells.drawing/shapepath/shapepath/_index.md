---
title: "ShapePath.ShapePath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ ShapePath. يهيئ مثيلًا جديدًا من الفئة ShapePath"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

يهيئ مثيلًا جديدًا من الفئة [`ShapePath`](../).

```csharp
public ShapePath()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أنشئ مسار شكل جديد باستخدام طريقة #ctor
                ShapePath shapePath = new ShapePath();

                // أضف مقاطع مسار لإنشاء شكل بسيط
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //إضافة شكل حر
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


