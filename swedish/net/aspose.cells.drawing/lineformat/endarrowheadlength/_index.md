---
title: "LineFormat.EndArrowheadLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat egenskap. Hämtar och anger slutpilens längdtyp för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

Hämtar och anger slutpilens längdtyp för linjen.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform och hämta formobjektet direkt
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Ange slutpilens längd
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // Spara arbetsboken
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


