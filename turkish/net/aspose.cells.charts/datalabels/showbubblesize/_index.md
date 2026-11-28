---
title: "DataLabels.ShowBubbleSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Belirli bir grafiğin veri etiketi yüzde değeri gösterim davranışını temsil eder. True yüzde değerini gösterir. False yüzde değerini gizler"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

Belirtilen bir grafiğin veri etiketi yüzde değerinin gösterim davranışını temsil eder. Doğru ise yüzde değeri gösterilir. Yanlış ise yüzde değeri gizlenir.

```csharp
public bool ShowBubbleSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // Bir balon grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe seri ekle
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Seri için balon boyutlarını ayarla
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // Serinin DataLabels'ına eriş
            DataLabels dataLabels = series.DataLabels;

            // ShowBubbleSize özelliğini göster
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


