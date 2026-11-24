---
title: "Enum CellBorderType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellBorderType-Enum. Enumeriert einen Zellenrandtyp"
type: docs
url: /de/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Enumeriert den Randtyp einer Zelle.

```csharp
public enum CellBorderType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DashDot | `9` | Stellt eine dünne Strich-Punkt-Linie dar. |
| DashDotDot | `11` | Stellt eine dünne Strich-Punkt-Punkt-Linie dar. |
| Dashed | `3` | Stellt eine gestrichelte Linie dar. |
| Dotted | `4` | Stellt eine gepunktete Linie dar. |
| Double | `6` | Stellt eine doppelte Linie dar. |
| Hair | `7` | Stellt eine Feinlinie dar. |
| MediumDashDot | `10` | Stellt eine mittlere Strich-Punkt-Linie dar. |
| MediumDashDotDot | `12` | Stellt eine mittlere Strich-Punkt-Punkt-Linie dar. |
| MediumDashed | `8` | Stellt eine mittlere gestrichelte Linie dar. |
| None | `0` | Stellt keine Linie dar. |
| Medium | `2` | Stellt eine mittlere Linie dar. |
| SlantedDashDot | `13` | Stellt eine schräg gestellte mittlere Strich-Punkt-Linie dar. |
| Thick | `5` | Stellt eine dicke Linie dar. |
| Thin | `1` | Stellt eine dünne Linie dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Bereich (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Rufen Sie den Stil des Bereichs ab
            Style style = workbook.CreateStyle();

            // Verschiedene Rahmenstile für den Bereich festlegen
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Den Stil auf den Bereich anwenden
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


