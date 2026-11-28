---
title: "Enum PrintSizeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PrintSizeType enum. Yazdırılan grafik boyutunu temsil eder"
type: docs
url: /tr/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Yazdırılan grafik boyutunu temsil eder.

```csharp
public enum PrintSizeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Full | `0` | Tam sayfa kullan. |
| Fit | `1` | Sayfaya sığacak şekilde ölçekle. |
| Custom | `2` | Özel. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarlayın
            chart.SetChartDataRange("A1:B4", true);

            // Grafik başlığını ayarla
            chart.Title.Text = "Sample Chart";

            // Grafiğin baskı boyutunu ayarla
            chart.PrintSize = PrintSizeType.Fit;

            // Çalışma kitabını kaydedin
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


