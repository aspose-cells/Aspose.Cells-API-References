---
title: "Line.WeightPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line-Eigenschaft. Liest oder setzt das Gewicht der Linie in Pixel"
type: docs
url: /de/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Ermittelt oder legt das Gewicht der Linie in Pixeln fest.

```csharp
public double WeightPx { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Ein Liniendiagramm hinzufügen
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurieren Sie Linieneigenschaften mit WeightPx
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


