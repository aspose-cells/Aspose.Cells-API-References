---
title: "Series.Border"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Stellt die Rahmenlinie eines Series‑Objekts dar"
type: docs
url: /de/net/aspose.cells.charts/series/border/
---
## Series.Border property

Stellt die Rahmenlinie eines Series-Objekts dar.

```csharp
public Line Border { get; }
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
    public class SeriesPropertyBorderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["A2"].PutValue("2020");
            worksheet.Cells["A3"].PutValue("2021");
            worksheet.Cells["A4"].PutValue("2022");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(7000);
            worksheet.Cells["B4"].PutValue(9000);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Seriendaten hinzufügen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte die erste Serie
            Series series = chart.NSeries[0];
            series.Name = "Sales Data";

            // Passen Sie die Rahmen‑Eigenschaften an
            series.Border.Color = System.Drawing.Color.Blue;
            series.Border.Weight = WeightType.MediumLine;
            series.Border.DashType = MsoLineDashStyle.Solid;
            series.Border.IsVisible = true;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


