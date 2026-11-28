---
title: "Series.CountOfDataValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Veri değerlerinin sayısını alır"
type: docs
url: /tr/net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Veri değerlerinin sayısını alır.

```csharp
public int CountOfDataValues { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyCountOfDataValuesDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
            }

            // Bir grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Veri aralığını kullanarak seri ekle
            chart.NSeries.Add("A1:A4", true);
            
            // İlk serideki veri değerlerinin sayısını göster
            Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


