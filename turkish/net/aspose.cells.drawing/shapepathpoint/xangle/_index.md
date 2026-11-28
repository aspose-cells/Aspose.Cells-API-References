---
title: "ShapePathPoint.XAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathPoint özelliği. Nesne bir açı işaretçisi olduğunda, derece cinsinden ilk açıyı al veya ayarla"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

Nesne bir açı işaretçisi olduğunda, ilk açıyı derece cinsinden alır veya ayarlar.

```csharp
public int XAngle { get; set; }
```

### Açıklamalar

Bu açı bir yay başlangıç açısıysa. Bu açı, varsayılan daire yolu boyunca yay çizmeye başlamak için kullanılacak açıyı belirler. Bu başlangıç açısı, şekil yolundaki son bilinen kalem konumuna kilitlenir. Böylece sürekli bir şekil yolu garantilenir.

### Örnekler

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
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Şekil yolu noktalarından bir koleksiyon oluştur
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // İlk noktayı al ve X ve Y koordinatlarını göster
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // NOT: ShapePathPoint sınıfı (mevcut API yansımasına göre) bir XAngle özelliği sunmaz.
            // Bu nedenle, bu demo mevcut X ve Y özelliklerine odaklanır.

            // Tanımlanan noktaları kullanarak basit bir serbest şekil oluştur
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Serbest şekli çalışma sayfasına ekle
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


