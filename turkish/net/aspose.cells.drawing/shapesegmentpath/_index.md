---
title: "Sınıf ShapeSegmentPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapeSegmentPath sınıfı. Serbest formun bir yolundaki segment yolunu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Serbest formun bir yolundaki segment yolunu temsil eder.

```csharp
public class ShapeSegmentPath
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Yol segmentindeki noktaları alır |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Yol segment tipi alır |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir serbest form şekli ekle
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Şeklin geometrik yolunu al
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // İlk segment yoluna eriş (varsa)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // ShapeSegmentPath özelliklerini göster
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Segment yolundaki noktalar arasında yinele
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


