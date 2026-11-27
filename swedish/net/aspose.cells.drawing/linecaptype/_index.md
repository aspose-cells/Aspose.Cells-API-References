---
title: "Enum LineCapType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.LineCapType enum. Representerar ändarna på en linje"
type: docs
url: /sv/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Representerar ändarna på en linje.

```csharp
public enum LineCapType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Square | `0` | Fyrkant sticker ut med halva linjebredden. |
| Round | `1` | Avrundade ändar. |
| Flat | `2` | Linjen slutar vid slutpunkten. |
| None | `3` | Ingen ända |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


