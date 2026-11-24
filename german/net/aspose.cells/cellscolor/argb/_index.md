---
title: "CellsColor.Argb"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor‑Eigenschaft. Gibt die Farbe aus einem 32‑Bit‑ARGB‑Wert zurück und legt sie fest."
type: docs
url: /de/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Liest und setzt die Farbe aus einem 32‑Bit‑ARGB‑Wert.

```csharp
public int Argb { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich und einen Stil.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Erstelle und konfiguriere CellsColor mithilfe der Argb‑Eigenschaft.
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Wende die Farbe auf den Stil an.
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Wende den Stil auf den Bereich an.
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Speichere die Arbeitsmappe
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


