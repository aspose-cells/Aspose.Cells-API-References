---
title: "Line.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Representerar linjens stil"
type: docs
url: /sv/net/aspose.cells.drawing/line/style/
---
## Line.Style property

Anger linjens stil.

```csharp
public LineType Style { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett exempeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Hämta den första serien och dess första punkt
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // Ställ in linjeegenskaper
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // Verifiera att stilen har satts
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


