---
title: "LineFormat.CapType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat egenskap. Anger avslutningskappar"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Anger slutkapparna.

```csharp
public LineCapType CapType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Ange linjeformatets egenskaper
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Spara arbetsboken
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


