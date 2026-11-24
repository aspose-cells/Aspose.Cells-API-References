---
title: "Marker.MarkerStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Marker-Eigenschaft. Gibt den Markierungsstil an. Gilt für ein Liniendiagramm, ein Streudiagramm oder ein Radar‑Diagramm"
type: docs
url: /de/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Stellt den Markerstil dar. Gilt für ein Liniendiagramm, ein Streudiagramm oder ein Radar-Diagramm.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Markierungsstil für die erste Serie festlegen
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // Speichere die Arbeitsmappe
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


