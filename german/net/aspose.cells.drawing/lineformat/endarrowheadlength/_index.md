---
title: "LineFormat.EndArrowheadLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Endpfeillängentyp der Linie zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

Ruft den Endpfeillängentyp der Linie ab und legt ihn fest.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Beispiele

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

            // Füge ein Linienobjekt hinzu und erhalte das Formobjekt direkt.
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Lege die Endpfeillänge fest
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


