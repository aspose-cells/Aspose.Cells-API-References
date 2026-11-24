---
title: "Klasse CellsColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellsColor‑Klasse. Stellt alle Farbtypen dar"
type: docs
url: /de/net/aspose.cells/cellscolor/
---
## CellsColor class

Stellt alle Farbtypen dar.

```csharp
public class CellsColor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Liest und setzt die Farbe aus einem 32‑Bit‑ARGB‑Wert. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Liest und setzt die RGB‑Farbe. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Liest und setzt den Farbindex in der Farbpalette. Gilt nur für indizierte Farben. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Liest und setzt die Farbe, die auf Zelle oder Form angewendet werden soll. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Liest die Themenfarbe. Gilt nur für den Typ Themenfarbe. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Liest und setzt die Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | Der Farbtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Setzen Sie den Farbton der Formfarbe |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Zellbereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Erstellen Sie eine CellsColor‑Instanz
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Setzen Sie Eigenschaften von CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Wenden Sie die CellsColor auf den Bereich an
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Speichere die Arbeitsmappe
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


