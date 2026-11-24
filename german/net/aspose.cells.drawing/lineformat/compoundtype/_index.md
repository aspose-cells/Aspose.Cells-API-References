---
title: "LineFormat.CompoundType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LineFormat-Eigenschaft. Gibt den zusammengesetzten Linientyp an"
type: docs
url: /de/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Gibt den Zeilenverbundtyp an.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Hole das Linienformat
            LineFormat lineFmt = line.Line;

            // Zusammengesetzten Typ festlegen
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


