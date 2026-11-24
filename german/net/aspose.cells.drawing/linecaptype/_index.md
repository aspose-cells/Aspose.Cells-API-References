---
title: "Aufzählung LineCapType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.LineCapType-Enum. Stellt die Enden einer Linie dar"
type: docs
url: /de/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Stellt die Enden (Caps) einer Linie dar

```csharp
public enum LineCapType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Square | `0` | Quadrat ragt um die halbe Linienbreite heraus. |
| Round | `1` | Abgerundete Enden. |
| Flat | `2` | Linie endet am Endpunkt. |
| None | `3` | Keine Endung |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


