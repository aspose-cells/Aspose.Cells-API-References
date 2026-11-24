---
title: "Series.Points"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt die Sammlung von Punkten einer Serie in einem Diagramm zurück"
type: docs
url: /de/net/aspose.cells.charts/series/points/
---
## Series.Points property

Liefert die Sammlung von Punkten einer Serie in einem Diagramm.

```csharp
public ChartPointCollection Points { get; }
```

### Hinweise

Wenn das Diagramm ein Pie‑of‑Pie oder Bar‑of‑Pie ist, ist der letzte Punkt ein anderer Punkt im ersten Kuchendiagramm.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greife auf die erste Serie und ihre Punkte zu
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Füge jedem Punkt Datenbeschriftungen hinzu
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


