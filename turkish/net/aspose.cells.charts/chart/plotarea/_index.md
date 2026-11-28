---
title: "Chart.PlotArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafiğin eksen işaretçi etiketlerini içeren çizim alanını alır"
type: docs
url: /tr/net/aspose.cells.charts/chart/plotarea/
---
## Chart.PlotArea property

Eksen işaret etiketi etiketlerini içeren grafiğin çizim alanını alır.

```csharp
public PlotArea PlotArea { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotAreaDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Çizim alanını özelleştir
            chart.PlotArea.Area.FillFormat.FillType = FillType.Solid;
            chart.PlotArea.Area.FillFormat.SolidFill.Color = Color.LightBlue;
            chart.PlotArea.Border.Color = Color.Black;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPlotAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


