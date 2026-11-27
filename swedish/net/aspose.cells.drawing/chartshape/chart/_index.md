---
title: "ChartShape.Chart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartShape-egenskap. Returnerar ett Chart-objekt som representerar diagrammet som finns i objektet"
type: docs
url: /sv/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Returnerar ett Chart-objekt som representerar diagrammet som finns i objektet.

```csharp
public Chart Chart { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta ChartShape-instansen
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Åtkomst till Chart-egenskapen (skrivskyddad)
            Chart accessedChart = chartShape.Chart;

            // Visa diagramegenskaper
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Ändra diagramegenskaper via Chart-objektet
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Ändra diagramtyp
            accessedChart.Type = ChartType.Pie;

            // Spara resultatet
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


