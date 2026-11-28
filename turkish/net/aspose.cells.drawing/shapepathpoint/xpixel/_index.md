---
title: "ShapePathPoint.XPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathPoint özelliği. Nesne bir konum koordinatı olduğunda, x koordinatını piksel cinsinden al veya ayarla"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

Nesne bir konum koordinatı olduğunda, x koordinatını piksel cinsinden alır veya ayarlar.

```csharp
public int XPixel { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
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

                // Koordinatlarla noktalar ekle
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // İlk noktaya eriş ve XPixel özelliğini göster
                ShapePathPoint firstPoint = pathPoints[0];

                // XPixel değerini göster (okuma işlemi)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // XPixel için yeni bir değer ayarla (okuma/yazma olduğu için)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Bir şekil yolu oluştur ve noktaları ekle
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // İkinci noktayı ekle
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

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
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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


