---
title: "Chart.PlotArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar diagrammets plotområde som inkluderar axelticketiketter"
type: docs
url: /sv/net/aspose.cells.charts/chart/plotarea/
---
## Chart.PlotArea property

Hämtar diagrammets plotområde som inkluderar axelns tick‑etiketter.

```csharp
public PlotArea PlotArea { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Anpassa plotområdet
            chart.PlotArea.Area.FillFormat.FillType = FillType.Solid;
            chart.PlotArea.Area.FillFormat.SolidFill.Color = Color.LightBlue;
            chart.PlotArea.Border.Color = Color.Black;

            // Spara arbetsboken
            workbook.Save("ChartPlotAreaDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


