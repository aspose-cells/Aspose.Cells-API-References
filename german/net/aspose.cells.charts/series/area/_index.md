---
title: "Series.Area"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Stellt den Hintergrundbereich des Series‑Objekts dar."
type: docs
url: /de/net/aspose.cells.charts/series/area/
---
## Series.Area property

Stellt den Hintergrundbereich des Series-Objekts dar.

```csharp
public Area Area { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyAreaDemo
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

            // Greife auf die erste Serie zu und setze die Flächentextur.
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Texture = TextureType.Stationery;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Area](../../../aspose.cells.drawing/area/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


