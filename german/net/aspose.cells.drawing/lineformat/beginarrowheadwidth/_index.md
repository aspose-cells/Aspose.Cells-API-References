---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den Anfangspfeilbreitentyp der Linie zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Ermittelt und setzt den Typ der Anfangspfeilbreite der Linie.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Linienformat-Eigenschaften festlegen
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


