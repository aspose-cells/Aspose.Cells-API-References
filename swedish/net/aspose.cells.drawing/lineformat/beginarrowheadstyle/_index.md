---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat egenskap. Hämtar och anger startpilens typ för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Hämtar och anger startpilens typ för linjen.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Ange startpilens stil
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Spara arbetsboken
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


