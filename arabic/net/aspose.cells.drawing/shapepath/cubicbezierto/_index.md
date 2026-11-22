---
title: "ShapePath.CubicBezierTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapePath. يضيف منحنى بيزيه مكعب إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. وحدة بكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

يضيف منحنى بيزيه مكعب إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ctrX1 | Single | الإحداثي السيني للنقطة التحكمية الأولى للمنحنى (الوحدة: بكسل). |
| ctrY1 | Single | الإحداثي الصادي للنقطة التحكمية الأولى للمنحنى (الوحدة: بكسل). |
| ctrX2 | Single | الإحداثي السيني للنقطة التحكمية الثانية للمنحنى (الوحدة: بكسل). |
| ctrY2 | Single | الإحداثي الصادي للنقطة التحكمية الثانية للمنحنى (الوحدة: بكسل). |
| endX | Single | الإحداثي السيني لنقطة النهاية للمنحنى (الوحدة: بكسل). |
| endY | Single | الإحداثي الصادي لنقطة النهاية للمنحنى (الوحدة: بكسل). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            //إنشاء مسار شكل جديد
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);


            //إضافة شكل حر
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // حفظ النتيجة
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


