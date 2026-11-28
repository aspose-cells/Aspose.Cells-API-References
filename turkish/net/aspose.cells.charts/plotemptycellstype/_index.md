---
title: "Enum PlotEmptyCellsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.PlotEmptyCellsType enum. Bir grafiğin tüm boş hücre çizim türlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Bir grafiğin tüm boş hücre grafik türlerini temsil eder.

```csharp
public enum PlotEmptyCellsType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| NotPlotted | `0` | Çizilmedi (boşluk bırak) |
| Zero | `1` | Sıfır |
| Interpolated | `2` | Aradeğerli |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarlayın
            chart.SetChartDataRange("A1:B5", true);

            // Grafiğin başlığını ayarlayın
            chart.Title.Text = "Plot Empty Cells Example";

            // Boş hücrelerin nasıl çizileceğini ayarlayın
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Çalışma kitabını kaydedin
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


