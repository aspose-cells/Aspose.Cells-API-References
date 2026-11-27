---
title: "Chart.ChartDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Representerar diagrammets datatabell"
type: docs
url: /sv/net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

Representerar diagrammets datatabell.

```csharp
public ChartDataTable ChartDataTable { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartDataTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Aktivera och anpassa datatabellen
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Ställ in datatabellens egenskaper
            dataTable.ShowLegendKey = true;
            dataTable.HasBorderHorizontal = true;
            dataTable.HasBorderVertical = true;
            dataTable.HasBorderOutline = true;
            dataTable.AutoScaleFont = true;
            dataTable.BackgroundMode = BackgroundMode.Opaque;

            // Anpassa datatabellens teckensnitt
            dataTable.Font.Name = "Arial";
            dataTable.Font.Size = 10;
            dataTable.Font.Color = Color.Blue;
            dataTable.Font.IsBold = true;

            // Anpassa datatabellens kanter
            dataTable.Border.Color = Color.Red;
            dataTable.Border.Style = LineType.Dash;
            dataTable.Border.Weight = WeightType.MediumLine;

            // Spara arbetsboken
            workbook.Save("ChartDataTableDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


