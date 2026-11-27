---
title: "Chart.PlotVisibleCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart‑egenskap. Anger om endast synliga celler ska plottas"
type: docs
url: /sv/net/aspose.cells.charts/chart/plotvisiblecells/
---
## Chart.PlotVisibleCells property

Anger om endast synliga celler ska plottas.

```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PlotVisibleCellsOnly‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["A4"].PutValue("Eve");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(90);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(95);

            // Dölj några rader
            worksheet.Cells.HideRow(2);
            worksheet.Cells.HideRow(3);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera PlotVisibleCells‑egenskapen
            chart.PlotVisibleCells = false; // Will not plot hidden cells
            // chart.PlotVisibleCells = true; // Plottar dolda celler (kommenterad för demo)

            // Spara arbetsboken
            workbook.Save("ChartPlotVisibleCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


