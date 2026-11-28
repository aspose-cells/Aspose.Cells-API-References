---
title: "ShapePathPoint.YPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathPoint özelliği. Nesne bir konum koordinatı olduğunda y koordinatını piksel cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

Nesne bir konum koordinatı olduğunda, y koordinatını piksel cinsinden alır veya ayarlar.

```csharp
public int YPixel { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir şekil yolu nokta koleksiyonu oluşturun
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Koordinatlarla bir nokta ekleyin
                pathPoints.Add(100, 50);

                // İlk noktaya erişin ve YPixel özelliğini gösterin
                ShapePathPoint firstPoint = pathPoints[0];

                // İlk YPixel değerini gösterin (okuma işlemi)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // YPixel için yeni bir değer ayarlayın (okuma/yazma olduğu için)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Bir şekil yolu oluşturun ve noktayı kullanın
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Çalışma sayfasına bir serbest form şekli ekle
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Çalışma kitabını kaydedin
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


