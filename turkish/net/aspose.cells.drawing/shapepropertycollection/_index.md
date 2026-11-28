---
title: "Sınıf ShapePropertyCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapePropertyCollection sınıfı. Bu sınıf, bir grafik öğesi veya şekil için görsel şekil özelliklerini belirtir."
type: docs
url: /tr/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

Bu sınıf, bir grafik öğesi veya şekil için görsel şekil özelliklerini belirtir.

```csharp
public class ShapePropertyCollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Grafik öğesi veya şekil için 3B şekil özelliklerini belirten bir [`Format3D`](./format3d/) nesnesini temsil eder. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Grafik öğesi veya şekil için parıltı etkisini belirten bir [`GlowEffect`](./gloweffect/) nesnesini temsil eder. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Grafik öğesi veya şekil için gölge etkisini belirten bir [`ShadowEffect`](./shadoweffect/) nesnesini temsil eder. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Kenarlar için uygulanacak bulanıklık yarıçapını puan (point) biriminde alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Şeklin 3B şekil özelliklerini temizler. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Şeklin parıltı etkisini temizler. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Grafik öğesi veya şeklin gölge etkisini temizler. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Şeklin 3B biçim verisine sahip olup olmadığını gösterir. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Şeklin parıltı etkisi verisine sahip olup olmadığını gösterir. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Şeklin gölge etkisi verisine sahip olup olmadığını gösterir. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePropertyCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir grafik oluşturun
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // İlk serinin şekil özelliklerine erişin
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // 3B biçimi ve köşe yuvarlamasını yapılandırın
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;
            
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Seri renklerini ayarlayın
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


