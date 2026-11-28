---
title: "DataLabels.IsNeverOverlap"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Pasta grafiğini görüntüye dönüştürürken veri etiketlerinin hiç çakışıp çakışmadığını gösterir. Not: Bu özellik yalnızca bir Pasta Grafiği görüntüye dönüştürüldüğünde anlamlıdır."
type: docs
url: /tr/net/aspose.cells.charts/datalabels/isneveroverlap/
---
## DataLabels.IsNeverOverlap property

Bir Pasta Grafiği görüntüsüne dönüştürülürken Datalabels'in hiç çakışıp çakışmadığını gösterir. Not: Bu özellik yalnızca bir Pasta Grafiği görüntüsüne dönüştürülürken anlamlıdır.

```csharp
public bool IsNeverOverlap { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsNeverOverlapDemo
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Veri etiketlerini etkinleştir
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Veri etiketlerini al ve IsNeverOverlap özelliğini ayarla
            DataLabels dataLabels = series.DataLabels;
            Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
            
            // IsNeverOverlap'i true olarak ayarla
            dataLabels.IsNeverOverlap = true;
            Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


