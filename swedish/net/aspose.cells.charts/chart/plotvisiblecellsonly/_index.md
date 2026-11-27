---
title: "Chart.PlotVisibleCellsOnly"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Anger om endast synliga celler ska plottas"
type: docs
url: /sv/net/aspose.cells.charts/chart/plotvisiblecellsonly/
---
## Chart.PlotVisibleCellsOnly property

Anger om endast synliga celler ska plottas.

```csharp
public bool PlotVisibleCellsOnly { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsOnlyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            
            // Dölj rad 3
            worksheet.Cells.Rows[2].IsHidden = true;
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ange PlotVisibleCellsOnly till false (standard är true)
            chart.PlotVisibleCellsOnly = false;
            
            // Spara arbetsboken
            workbook.Save("ChartPlotVisibleCellsOnlyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


