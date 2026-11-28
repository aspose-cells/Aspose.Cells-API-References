---
title: "Enum BevelPresetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.BevelPresetType enum. 3B'de bir şekle uygulanabilen bir köşe tipinin ön ayarını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

3B'de bir şekle uygulanabilen bir köşe tipi için bir ön ayarı temsil eder.

```csharp
public enum BevelPresetType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Kenarsız |
| Angle | `1` | Açı |
| ArtDeco | `2` | Art deco |
| Circle | `3` | Daire |
| Convex | `4` | Konveks |
| CoolSlant | `5` | Serin eğim |
| Cross | `6` | Çapraz |
| Divot | `7` | Çökük |
| HardEdge | `8` | Keskin kenar |
| RelaxedInset | `9` | Rahat iç kenar |
| Riblet | `10` | Kaburga |
| Slope | `11` | Eğim |
| SoftRound | `12` | Yumuşak yuvarlak |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafiğin başlığına erişin ve metnini ayarlayın
            chart.Title.Text = "Sample Chart with Bevel";

            // Grafiğin çizim alanına erişin
            PlotArea plotArea = chart.PlotArea;

            // Çizim alanının şekil özelliklerine erişin
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // 3B format özelliklerine erişin
            Format3D format3D = shapeProperties.Format3D;

            // Üst köşe özelliklerine erişin
            Bevel topBevel = format3D.TopBevel;

            // Köşe tipini "Angle" olarak ayarlayın
            topBevel.Type = BevelPresetType.Angle;

            // Köşenin genişliğini ve yüksekliğini ayarlayın
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Çalışma kitabını kaydedin
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


