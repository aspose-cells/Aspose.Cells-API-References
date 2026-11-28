---
title: "Series.IsVerticalValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Veri kaynağının dikey olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Veri kaynağının dikey olup olmadığını gösterir.

```csharp
public bool IsVerticalValues { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Dikey değerlerle seri ekle
            chart.NSeries.Add("A1:B10", true);
            
            // IsVerticalValues özelliğini göster (yalnızca okunabilir)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // Yönelimi değiştirmek için seriyi farklı parametrelerle yeniden oluşturmalıyız
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


