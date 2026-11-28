---
title: "Enum LegendPositionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.LegendPositionType enum. Lejant konum türlerini sıralar"
type: docs
url: /tr/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Lejant konum türlerini listeler.

```csharp
public enum LegendPositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Bottom | `0` | Lejantı grafiğin çizim alanının altına gösterir. |
| Corner | `1` | Lejantı grafiğin çizim alanının köşesinde gösterir. |
| Left | `4` | Lejantı grafiğin çizim alanının solunda gösterir. |
| NotDocked | `7` | Lejantın yerleştirilmediğini gösterir. |
| Right | `3` | Lejantı grafiğin çizim alanının sağında gösterir. |
| Top | `2` | Lejantı grafiğin çizim alanının üstünde gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Çalışma sayfasına bir sütun grafiği ekle
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Grafiğin açıklamasına erişin
            Legend legend = chart.Legend;

            // Lejantın konumunu grafiğin soluna ayarla
            legend.Position = LegendPositionType.Left;

            // Lejant için ek özellikleri ayarla
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Çalışma kitabını kaydedin
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


