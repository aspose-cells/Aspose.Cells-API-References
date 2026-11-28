---
title: "ShapePath.ArcTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath yöntemi. Mevcut şekle eliptik bir yay ekler. Başlangıç noktası, mevcut şeklin son noktasıdır"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Mevcut şekle eliptik bir yay ekler. Başlangıç noktası, mevcut şeklin son noktasıdır.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| wR | Single | Yayın çizildiği elipsin dikdörtgen alanının yarı genişliği (Birim: Piksel). |
| hR | Single | Yayın çizildiği elipsin dikdörtgen alanının yarı yüksekliği (Birim: Piksel). |
| stAng | Single | Yayın başlangıç açısı, x ekseninden saat yönünde derece cinsinden ölçülür (Birim: Derece). Bu açı, yay çizilirken başlangıç konumu olarak kullanılacak varsayılan daire yolundaki açıyı belirler. Bu başlangıç açısı, şekil yolundaki son bilinen kalem konumuna kilitlenir. Böylece kesintisiz bir şekil yolu garantilenir. |
| swAng | Single | Bir yay için salınım açısı. Bu açı, yayının varsayılan daire yolu boyunca açı olarak ne kadar uzatılacağını belirler. Başlangıç açısından uzatma her zaman varsayılan daire etrafında saat yönünde olur. (Birim: Derece) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //Yeni bir şekil yolu oluştur
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

            //Yeni bir şekil yolu oluştur
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);

            Workbook workbook = new Workbook();

            //serbest form ekle
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Sonucu kaydet
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


