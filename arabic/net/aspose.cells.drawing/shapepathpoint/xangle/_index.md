---
title: "ShapePathPoint.XAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePathPoint. عندما يكون الكائن علامة زاوية احصل على أو اضبط الزاوية الأولى بالدرجات"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

عندما يكون الكائن علامة زاوية، احصل أو اضبط الزاوية الأولى بالدرجات.

```csharp
public int XAngle { get; set; }
```

### ملاحظات

إذا كانت هذه الزاوية هي الزاوية الابتدائية لقوس. ستحدد هذه الزاوية أي زاوية على مسار الدائرة المفترض سيتم استخدامها كنقطة بدء لرسم القوس. سيتم قفل زاوية البدء هذه إلى آخر موضع قلم معروف في مسار الشكل. وبالتالي يضمن مسار شكل مستمر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة من نقاط مسار الشكل
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // استرجاع النقطة الأولى وعرض إحداثيات X و Y الخاصة بها
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // ملاحظة: فئة ShapePathPoint (وفقًا للانعكاس الحالي لواجهة برمجة التطبيقات) لا تعرض خاصية XAngle.
            // لذلك، يركز هذا العرض التوضيحي على خصائص X و Y المتاحة.

            // بناء شكل حر بسيط باستخدام النقاط المحددة
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // إضافة الشكل الحر إلى ورقة العمل
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // احفظ المصنف
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


