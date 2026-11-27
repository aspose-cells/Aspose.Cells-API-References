---
title: "LineFormat.EndArrowheadStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat‑egenskap. Hämtar och anger slutpiltypen för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Hämtar och anger slutpilens typ för linjen.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Hämta linjeformatet
            LineFormat lineFmt = line.Line;

            // Ställ in stil för slutpilhuvudet
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Spara arbetsboken
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


