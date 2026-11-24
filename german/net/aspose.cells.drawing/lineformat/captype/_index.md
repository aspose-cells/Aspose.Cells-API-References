---
title: "LineFormat.CapType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt die Endkappen an."
type: docs
url: /de/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Gibt die Endkappen an.

```csharp
public LineCapType CapType { get; set; }
```

### Beispiele

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

            // Eine Linienform hinzufügen
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Linienformat-Eigenschaften festlegen
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


