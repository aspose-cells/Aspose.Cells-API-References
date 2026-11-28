---
title: "Chart.FilteredNSeries"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafikte filtrelenen veri serilerini temsil eden bir SeriesCollection koleksiyonu alır"
type: docs
url: /tr/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Grafikte filtrelenen veri serilerini temsil eden bir [`SeriesCollection`](../../seriescollection/) koleksiyonu alır.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekle ve bazı serileri filtreli olarak ayarla
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Bazı serileri filtrele (Seri 2'yi gizle)
            chart.NSeries[1].IsFiltered = true;

            // Filtrelenmiş seri koleksiyonuna eriş
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Çalışma kitabını kaydedin
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


