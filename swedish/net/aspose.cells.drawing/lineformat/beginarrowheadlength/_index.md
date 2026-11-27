---
title: "LineFormat.BeginArrowheadLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat egenskap. Hämtar och anger startpilens längdtyp för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Hämtar och ställer in startpilens längdtyp för linjen.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Ange startpilens längd
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Spara arbetsboken
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


