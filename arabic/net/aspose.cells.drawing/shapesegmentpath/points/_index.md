---
title: "ShapeSegmentPath.Points"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeSegmentPath. يحصل على النقاط في مقطع المسار"
type: docs
url: /ar/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

يحصل على النقاط في جزء المسار

```csharp
public ShapePathPointCollection Points { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {// Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // ابدأ مسارًا جديدًا
            path.MoveTo(10, 10);

            // ارسم مقطع خط
            path.LineTo(100, 100);

            // الوصول إلى خاصية PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // الوصول إلى مسار المقطع الأول
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // عرض معلومات النقاط
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //إضافة شكل حر
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // احفظ المصنف
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


