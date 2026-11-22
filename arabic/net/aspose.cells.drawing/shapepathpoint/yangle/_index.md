---
title: "ShapePathPoint.YAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePathPoint. عندما يكون الكائن علامة زاوية، احصل أو اضبط الزاوية الثانية بالدرجات"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

عندما يكون الكائن علامة زاوية، احصل أو اضبط الزاوية الثانية بالدرجات.

```csharp
public int YAngle { get; set; }
```

### ملاحظات

إذا كانت هذه الزاوية هي زاوية التأرجح لقوس. ستحدد هذه الزاوية مدى الامتداد الزاوي على طول مسار الدائرة المفترض للقوس. الامتداد من زاوية البداية سيكون دائمًا في الاتجاه الساعي للساعة حول الدائرة المفترضة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء مجموعة نقاط مسار الشكل
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // إضافة نقاط مع علامات الزاوية (باستخدام XAngle و YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // عرض قيمة YAngle
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // إنشاء نقطة أخرى بزاويا مختلفة
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // عرض قيمة YAngle
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // إنشاء مسار شكل وإضافة قوس باستخدام علامات الزاوية
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

                // إضافة شكل حر إلى ورقة العمل
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // احفظ المصنف
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


