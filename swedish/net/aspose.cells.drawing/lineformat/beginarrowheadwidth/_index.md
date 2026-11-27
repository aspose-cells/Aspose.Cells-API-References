---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat-egenskap. Hämtar och anger startpilens breddtyp för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Hämtar och anger startpilens breddtyp för linjen.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Ange linjeformatets egenskaper
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Spara arbetsboken
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


