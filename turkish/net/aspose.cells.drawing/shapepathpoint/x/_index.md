---
title: "ShapePathPoint.X"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathPoint özelliği. Bu konum koordinatı için x koordinatını alır ve ayarlar. Birim EMU"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpoint/x/
---
## ShapePathPoint.X property

Bu konum koordinatı için x koordinatını alır ve ayarlar. Birim EMU.

```csharp
[Obsolete("Use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int X { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ShapePathPoint.XPixel ve ShapePathPoint.XAngle özelliklerini kullanın. Bu özellik, Ağustos 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil yolu nokta koleksiyonu oluşturun ve nokta ekleyin
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Noktalara Item özelliğini kullanarak erişin
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Noktalara dayanarak bir şekil yolu oluşturun
            ShapePath path = new ShapePath();

            // Başlangıç noktasına git
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Yapılandırılmış yol ile serbest şekil ekleyin
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ShapePathPointXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


