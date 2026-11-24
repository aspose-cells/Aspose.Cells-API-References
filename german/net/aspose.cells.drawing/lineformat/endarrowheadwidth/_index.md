---
title: "LineFormat.EndArrowheadWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Endpfeilbreitentyp der Linie zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Ruft den Endpfeilbreitentyp der Linie ab und legt ihn fest.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Beispiele

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

            // Eine Linienform hinzufügen
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Hole das Linienformat
            LineFormat lineFmt = line.Line;

            // Endpfeilbreite festlegen
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


