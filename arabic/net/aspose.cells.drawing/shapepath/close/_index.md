---
title: "ShapePath.Close"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapePath. تغلق الشكل الحالي وتبدأ شكلاً جديدًا. إذا كان الشكل الحالي يحتوي على سلسلة من الخطوط والمنحنيات المتصلة، فإن الطريقة تغلق الحلقة بربط خط من نقطة النهاية إلى نقطة البداية."
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

يغلق الشكل الحالي ويبدأ شكلًا جديدًا. إذا كان الشكل الحالي يحتوي على سلسلة من الخطوط والمنحنيات المتصلة، فإن الطريقة تغلق الحلقة بربط خط من نقطة النهاية إلى نقطة البداية.

```csharp
public void Close()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //إنشاء مسار شكل جديد
                ShapePath shapePath = new ShapePath();
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // إغلاق المسار
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // إغلاق المسار
                shapePath.Close();

                //إضافة شكل حر
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // احفظ المصنف
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


