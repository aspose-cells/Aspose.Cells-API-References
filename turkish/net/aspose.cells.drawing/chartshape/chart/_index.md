---
title: "ChartShape.Chart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartShape özelliği. Nesne içinde bulunan grafiği temsil eden bir Chart nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Nesnede bulunan grafiği temsil eden bir Chart nesnesi döndürür.

```csharp
public Chart Chart { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ChartShape örneğini alın
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Chart özelliğine erişin (yalnızca okunur)
            Chart accessedChart = chartShape.Chart;

            // Grafik özelliklerini görüntüleyin
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Chart nesnesi aracılığıyla grafik özelliklerini değiştirin
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Grafik türünü değiştirin
            accessedChart.Type = ChartType.Pie;

            // Sonucu kaydet
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


