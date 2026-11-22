---
title: "ShapePath.MoveTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapePath. تبدأ شكلاً جديدًا من النقطة المحددة دون إغلاق الشكل الحالي. جميع النقاط اللاحقة التي تُضاف إلى المسار تُضاف إلى هذا الشكل الجديد. الوحدة: بكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

يبدأ شكلًا جديدًا من النقطة المحددة دون إغلاق الشكل الحالي. جميع النقاط اللاحقة المضافة إلى المسار تُضاف إلى هذا الشكل الجديد. الوحدة: بكسل.

```csharp
public void MoveTo(float x, float y)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| x | Single | الإحداثي السيني لنقطة البداية للشكل (الوحدة: بكسل). |
| y | Single | الإحداثي الصادي لنقطة البداية للشكل (الوحدة: بكسل). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
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

                // الانتقال إلى النقطة البداية
                shapePath.MoveTo(10, 10);

                // استدعاء طريقة LineTo مع معلمات (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //إضافة شكل حر
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // حفظ النتيجة
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


