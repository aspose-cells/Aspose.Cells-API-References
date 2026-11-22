---
title: "ShapePath.ArcTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapePath. تُضيف قوسًا بيضاويًا إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

يضيف قوسًا بيضاويًا إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| wR | Single | نصف عرض المنطقة المستطيلة للبيضاوي التي ترسم القوس (الوحدة: بكسل). |
| hR | Single | نصف ارتفاع المنطقة المستطيلة للبيضاوي التي ترسم القوس (الوحدة: بكسل). |
| stAng | Single | زاوية البداية للقوس، تُقاس بالدرجات في اتجاه عقارب الساعة من المحور السيني (الوحدة: درجة). تحدد هذه الزاوية أي زاوية على مسار الدائرة المفترض ستُستخدم كنقطة بدء لرسم القوس. سيتم تثبيت زاوية البداية هذه على آخر موضع قلم معروف في مسار الشكل. وبالتالي يضمن مسار شكل مستمر. |
| swAng | Single | زاوية الانحراف للقوس. تحدد هذه الزاوية مدى الامتداد الزاوي على مسار الدائرة المفترض. الامتداد من زاوية البداية سيكون دائمًا في اتجاه عقارب الساعة حول الدائرة المفترض (الوحدة: درجة). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //إنشاء مسار شكل جديد
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

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

            Workbook workbook = new Workbook();

            //إضافة شكل حر
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // حفظ النتيجة
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


