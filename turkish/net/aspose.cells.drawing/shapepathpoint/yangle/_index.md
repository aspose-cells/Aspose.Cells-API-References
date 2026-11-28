---
title: "ShapePathPoint.YAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathPoint özelliği. Nesne bir açı işareti olduğunda ikinci açıyı derece cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

Nesne bir açı işaretçisi olduğunda, ikinci açıyı derece cinsinden alır veya ayarlar.

```csharp
public int YAngle { get; set; }
```

### Açıklamalar

Eğer bu açı bir yay için salınım açısı ise. Bu açı, yay boyunca varsayılan daire yolunda açı olarak ne kadar uzatılacağını belirler. Başlangıç açısından uzatma her zaman varsayılan daire etrafında saat yönünde olacaktır.

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir şekil yolu nokta koleksiyonu oluşturun
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Açı işaretleriyle (XAngle ve YAngle kullanarak) noktalar ekleyin
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // YAngle değerini gösterin
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Farklı açılarla başka bir nokta oluştur
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // YAngle değerini gösterin
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Bir şekil yolu oluştur ve açı işaretçileri kullanarak yay ekle
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

                // Çalışma sayfasına serbest biçimli şekil ekle
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


