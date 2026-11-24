---
title: "LineFormat.BeginArrowheadLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Anfangspfeillängentyp der Linie zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Ermittelt und setzt den Typ der Anfangspfeillänge der Linie.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Lege die Anfangspfeillänge fest
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


