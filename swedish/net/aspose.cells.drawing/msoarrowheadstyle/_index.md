---
title: "Enum MsoArrowheadStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoArrowheadStyle-enum. Enumererar linjeändningstypen för formens kantlinje"
type: docs
url: /sv/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Enumererar linjeändans typ för formens kantlinje.

```csharp
public enum MsoArrowheadStyle
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen linjeändtyp. |
| Arrow | `1` | Pillinjeändtyp. |
| ArrowStealth | `2` | Pil Stealth linjeändtyp. |
| ArrowDiamond | `3` | Pil Diamant linjeändtyp. |
| ArrowOval | `4` | Pil Oval linjeändtyp. |
| ArrowOpen | `5` | Pil Öppen linjeändtyp. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Ställ in linjeegenskaper
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Ställ in pilspetsstilar
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Spara arbetsboken
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


