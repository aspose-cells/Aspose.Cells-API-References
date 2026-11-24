---
title: "Enum BorderType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.BorderType Enum. Enumeriert die Arten von Randlinien und Diagonallinien"
type: docs
url: /de/net/aspose.cells/bordertype/
---
## BorderType enumeration

Enumeriert die Typen von Randlinien und Diagonallinien.

```csharp
[Flags]
public enum BorderType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LeftBorder | `1` | Stellt die linke Randlinie dar. |
| RightBorder | `2` | Stellt die rechte Randlinie dar. |
| TopBorder | `4` | Stellt die obere Randlinie dar. |
| BottomBorder | `8` | Stellt die untere Randlinie dar. |
| DiagonalDown | `10` | Stellt die diagonale Linie von oben links nach unten rechts dar. |
| DiagonalUp | `20` | Stellt die diagonale Linie von unten links nach oben rechts dar. |
| Vertical | `40` | Nur für dynamische Stile, wie bedingte Formatierung, Pivot‑Tabelle. |
| Horizontal | `80` | Nur für dynamische Stile, wie bedingte Formatierung, Pivot‑Tabelle. |
| SideBorders | `F` | Gibt die vier Seitenränder an: LeftBorder, RightBorder, TopBorder und BottomBorder. |
| Diagonal | `30` | Spezielle Kombination mehrerer Ränder zur Benutzerfreundlichkeit für einige APIs. Gibt die diagonalen Ränder DiagonalUp und DiagonalDown an. |
| DynamicStyleBorders | `C0` | Gibt Vertikal und Horizontal des dynamischen Stils an. |
| None | `0` | Es wurde kein Rand angegeben. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            // Erstelle einen Zellbereich
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Erstellen Sie ein Stilobjekt
            Style style = workbook.CreateStyle();
            // Setze die Ränder für den Bereich
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Den Stil auf den Bereich anwenden
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Speichere die Arbeitsmappe
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


