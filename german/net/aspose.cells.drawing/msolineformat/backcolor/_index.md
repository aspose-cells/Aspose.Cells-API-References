---
title: "MsoLineFormat.BackColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormat-Eigenschaft. Gibt die Hintergrundfarbe der Rahmenlinie zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Liest und setzt die Hintergrundfarbe der Randlinie.

```csharp
public Color BackColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Linieneigenschaften festlegen
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Speichere die Arbeitsmappe
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


