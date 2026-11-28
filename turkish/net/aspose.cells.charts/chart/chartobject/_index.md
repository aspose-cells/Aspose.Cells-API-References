---
title: "Chart.ChartObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. chartShape'ı temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chart/chartobject/
---
## Chart.ChartObject property

chartShape öğesini temsil eder;

```csharp
public ChartShape ChartObject { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ChartObject özelliklerini göster
            chart.ChartObject.Placement = PlacementType.Move;
            chart.ChartObject.X = 100;
            chart.ChartObject.Y = 200;
            chart.ChartObject.Width = 400;
            chart.ChartObject.Height = 300;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartObjectDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartShape](../../../aspose.cells.drawing/chartshape/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


