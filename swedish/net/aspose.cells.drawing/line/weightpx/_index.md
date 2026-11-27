---
title: "Line.WeightPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Hämtar eller anger linjens tjocklek i pixelenheter"
type: docs
url: /sv/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Hämtar eller anger linjens vikt i pixlar.

```csharp
public double WeightPx { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Lägg till exempeldata
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Lägg till ett linjediagram
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera linjeegenskaper med WeightPx
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Spara arbetsboken
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


