---
title: "Series.ShowNegativeBubbles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Seri özelliği. Grafik grubunda negatif balonlar gösteriliyorsa doğru. Yalnızca balon grafiklerinde geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

Grafik grubunda negatif baloncuklar gösteriliyorsa doğru. Yalnızca baloncuk grafiklerinde geçerlidir.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Balon grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // Bir balon grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // İlk seriye erişin ve ShowNegativeBubbles özelliğini ayarlayın
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


