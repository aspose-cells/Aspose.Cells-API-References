---
title: "Line.JoinType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Anger sammankopplingsändar"
type: docs
url: /sv/net/aspose.cells.drawing/line/jointype/
---
## Line.JoinType property

Specificerar sammankopplingsändarna.

```csharp
public LineJoinType JoinType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ange linjeanslutningstyp
            Line majorGridLines = chart.ValueAxis.MajorGridLines;
            majorGridLines.JoinType = LineJoinType.Round;

            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Se även

* enum [LineJoinType](../../linejointype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


