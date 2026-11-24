---
title: "Aufzählung PlotEmptyCellsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.PlotEmptyCellsType enum. Stellt alle leeren Zellen-Typen eines Diagramms dar"
type: docs
url: /de/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Stellt alle leeren Zellentypen eines Diagramms dar.

```csharp
public enum PlotEmptyCellsType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| NotPlotted | `0` | Nicht dargestellt (Lücke lassen) |
| Zero | `1` | Null |
| Interpolated | `2` | Interpoliert |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich für das Diagramm fest
            chart.SetChartDataRange("A1:B5", true);

            // Setze den Titel des Diagramms
            chart.Title.Text = "Plot Empty Cells Example";

            // Festlegen, wie leere Zellen dargestellt werden
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Speichere die Arbeitsmappe
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


