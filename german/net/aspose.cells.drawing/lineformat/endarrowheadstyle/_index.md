---
title: "LineFormat.EndArrowheadStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Endpfeiltyp der Linie zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Ruft den Endpfeiltyp der Linie ab und legt ihn fest.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Hole das Linienformat
            LineFormat lineFmt = line.Line;

            // Setzen Sie den Endpfeilstil
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


