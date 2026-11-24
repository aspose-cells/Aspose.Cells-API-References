---
title: "Line.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Linieneigenschaft. Stellt den Stil der Linie dar"
type: docs
url: /de/net/aspose.cells.drawing/line/style/
---
## Line.Style property

Stellt den Stil der Linie dar.

```csharp
public LineType Style { get; set; }
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
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle ein Beispiel-Diagramm
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Hole die erste Serie und ihren ersten Punkt
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // Linieneigenschaften festlegen
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // Überprüfe, ob der Stil gesetzt wurde
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


