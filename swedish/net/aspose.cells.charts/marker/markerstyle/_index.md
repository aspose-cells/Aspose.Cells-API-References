---
title: "Marker.MarkerStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Marker-egenskap. Representerar markörstilen. Gäller för ett linjediagram, ett spridningsdiagram eller ett radardiagram"
type: docs
url: /sv/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Representerar markörstilen. Gäller för ett linjediagram, ett spridningsdiagram eller ett radardiagram.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Ställ in markörstilen för den första serien
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // Spara arbetsboken
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


