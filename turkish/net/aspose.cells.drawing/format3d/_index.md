---
title: "Format3D sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Format3D sınıfı. Bu sınıf, bir grafik öğesi veya şekil için 3B şekil özelliklerini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/format3d/
---
## Format3D class

Bu sınıf, bir grafik öğesi veya şekil için 3B şekil özelliklerini belirtir.

```csharp
public class Format3D
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Aydınlatma açısını alır ve ayarlar. Aralık 0 ile 359,9 derece arasındadır. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Şeklin sahnesine uygulanacak aydınlatma tipini alır ve ayarlar. Varsayılan değer LightRigType.ThreePoint'tir. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Aydınlatma özellikleriyle birleştirilerek bir şeklin son görünüm ve hissini sağlayan malzeme tipini alır ve ayarlar. Varsayılan değer PresetMaterialType.WarmMatte'dir. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Şeklin üst veya ön yüzünde bir köşe (bevel) tanımlamaya ilişkin özellikleri tutan [`Bevel`](../bevel/) nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Şeklin üst köşe verisine sahip olup olmadığını gösterir. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Grafiğe seri ekle
            chart.NSeries.Add("A1:A4", true);

            // İlk seriye erişin
            Series series = chart.NSeries[0];

            // Serinin 3B formatına eriş
            Format3D format3D = series.ShapeProperties.Format3D;

            // 3B biçim özelliklerini ayarlayın
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Şeklin üst köşe verisine sahip olup olmadığını kontrol edin
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


