---
title: "Series.XValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bu grafik serisinin X değerlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Bu grafik serisinin X değerlerini temsil eder.

```csharp
public string XValues { get; set; }
```

### Açıklamalar

Yalnızca Scatter ve Bubble grafikler için. Diğer grafik türleri için lütfen [`CategoryData`](../../seriescollection/categorydata/) kullanın. [`CategoryValues`](../categoryvalues/) bu serinin gerçek kategori değerlerini almak için kullanılır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Scatter grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // XValues ve Values ile seri ekleyin
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


