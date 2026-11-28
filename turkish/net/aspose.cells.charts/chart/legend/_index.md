---
title: "Chart.Legend"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafik başlığını alır."
type: docs
url: /tr/net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

Grafik açıklamasını alır.

```csharp
public Legend Legend { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyLegendDemo
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

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Başlığı özelleştir
            chart.Legend.IsAutomaticSize = false;
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.Width = 400;
            chart.Legend.Height = 50;
            chart.Legend.Font.Size = 12;
            chart.Legend.Font.IsBold = true;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartLegendDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


