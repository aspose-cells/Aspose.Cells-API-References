---
title: "Series.PlotOnSecondAxis"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt an, ob diese Serie auf der zweiten Werteachse geplottet wird"
type: docs
url: /de/net/aspose.cells.charts/series/plotonsecondaxis/
---
## Series.PlotOnSecondAxis property

Gibt an, ob diese Serie auf der sekundären Wertachse dargestellt wird.

```csharp
public bool PlotOnSecondAxis { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPlotOnSecondAxisDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Legen Sie fest, dass die erste Serie auf der sekundären Achse geplottet wird
            chart.NSeries[0].PlotOnSecondAxis = true;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyPlotOnSecondAxisDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


