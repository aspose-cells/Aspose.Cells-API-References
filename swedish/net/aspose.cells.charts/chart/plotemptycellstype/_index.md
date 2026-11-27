---
title: "Chart.PlotEmptyCellsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart‑egenskap. Hämtar och anger hur tomma celler ska plottas"
type: docs
url: /sv/net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Hämtar och anger hur tomma celler ska plottas.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med några tomma celler
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            // B3 lämnas tom
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera PlotEmptyCellsType‑egenskapen
            chart.PlotEmptyCellsType = Aspose.Cells.Charts.PlotEmptyCellsType.Zero;
            Console.WriteLine("PlotEmptyCellsType set to: " + chart.PlotEmptyCellsType);

            // Spara arbetsboken
            workbook.Save("PlotEmptyCellsTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


