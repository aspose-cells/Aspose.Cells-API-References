---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Anfangspfeiltyp der Linie zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Ermittelt und setzt den Typ des Anfangspfeils der Linie.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Lege den Anfangspfeilstil fest
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


