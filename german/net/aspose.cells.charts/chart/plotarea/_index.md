---
title: "Chart.PlotArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt den Plotbereich des Diagramms zurück, der Achsenbeschriftungen enthält"
type: docs
url: /de/net/aspose.cells.charts/chart/plotarea/
---
## Chart.PlotArea property

Liest den Zeichenbereich des Diagramms, der Achsenbeschriftungen enthält.

```csharp
public PlotArea PlotArea { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Plotbereich anpassen
            chart.PlotArea.Area.FillFormat.FillType = FillType.Solid;
            chart.PlotArea.Area.FillFormat.SolidFill.Color = Color.LightBlue;
            chart.PlotArea.Border.Color = Color.Black;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPlotAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


