---
title: "DataLabels.ShowPercentage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Belirli bir grafiğin veri etiketi yüzde değeri gösterim davranışını temsil eder. True yüzde değerini gösterir. False gizlemek için."
type: docs
url: /tr/net/aspose.cells.charts/datalabels/showpercentage/
---
## DataLabels.ShowPercentage property

Belirtilen bir grafiğin veri etiketi yüzde değerinin gösterim davranışını temsil eder. Doğru ise yüzde değeri gösterilir. Yanlış ise gizlenir.

```csharp
public bool ShowPercentage { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowPercentageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Veri etiketlerini etkinleştir ve yüzdeyi göster
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowPercentage = true;
            dataLabels.ShowValue = false;

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsShowPercentageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


