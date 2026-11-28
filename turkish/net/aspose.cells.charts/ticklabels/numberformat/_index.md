---
title: "TickLabels.NumberFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. TickLabels nesnesi için biçim dizesini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

TickLabels nesnesi için biçim dizesini temsil eder.

```csharp
public string NumberFormat { get; set; }
```

### Açıklamalar

Biçim dizesi, bir hücreye uygulanan özel biçim dizesi ayarı ile aynıdır. Örneğin, "$0".

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Bir grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A2:A4", true);

            // Değer ekseni tick etiketleri için sayı biçimini ayarla
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


