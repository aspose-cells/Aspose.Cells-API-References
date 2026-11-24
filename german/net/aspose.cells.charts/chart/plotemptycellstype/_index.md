---
title: "Chart.PlotEmptyCellsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Eigenschaft. Gibt an, wie leere Zellen geplottet werden, und legt dies fest."
type: docs
url: /de/net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Liest und setzt, wie leere Zellen geplottet werden.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Beispiele

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
            
            // Beispieldaten mit einigen leeren Zellen hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            // B3 bleibt leer
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Diagramm hinzufügen
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Datenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstration der PlotEmptyCellsType‑Eigenschaft
            chart.PlotEmptyCellsType = Aspose.Cells.Charts.PlotEmptyCellsType.Zero;
            Console.WriteLine("PlotEmptyCellsType set to: " + chart.PlotEmptyCellsType);

            // Speichere die Arbeitsmappe
            workbook.Save("PlotEmptyCellsTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


