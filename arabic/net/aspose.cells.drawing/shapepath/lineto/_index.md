---
title: "ShapePath.LineTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapePath. تُضيف مقطع خط إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. وحدة بكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

يضيف مقطع خط إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل.

```csharp
public void LineTo(float x, float y)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| x | Single | الإحداثي السيني لنقطة النهاية لمقطع الخط (الوحدة: بكسل). |
| y | Single | الإحداثي الصادي لنقطة النهاية لمقطع الخط (الوحدة: بكسل). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
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

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


