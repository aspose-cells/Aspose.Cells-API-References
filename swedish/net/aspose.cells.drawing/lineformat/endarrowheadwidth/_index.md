---
title: "LineFormat.EndArrowheadWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat-egenskap. Hämtar och anger slutpilens breddtyp för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Hämtar och anger slutpilens breddtyp för linjen.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Hämta linjeformatet
            LineFormat lineFmt = line.Line;

            // Ange slutpilens bredd
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Spara arbetsboken
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


