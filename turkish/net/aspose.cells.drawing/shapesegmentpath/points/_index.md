---
title: "ShapeSegmentPath.Points"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeSegmentPath özelliği. Yol segmentindeki noktaları alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Yol segmentindeki noktaları alır

```csharp
public ShapePathPointCollection Points { get; }
```

### Örnekler

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

            // Yeni bir yol başlat
            path.MoveTo(10, 10);

            // Bir çizgi segmenti çiz.
            path.LineTo(100, 100);

            // PathSegementList özelliğine eriş
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // İlk segment yoluna eriş
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Nokta bilgilerini göster
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //serbest form ekle
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


