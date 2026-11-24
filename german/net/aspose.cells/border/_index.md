---
title: "Klasse Border"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Border Klasse. Kapselt das Objekt, das den Zellenrand darstellt."
type: docs
url: /de/net/aspose.cells/border/
---
## Border class

Kapselt das Objekt, das den Zellenrand darstellt.

```csharp
public class Border
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Liest und setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Liest oder setzt die Farbe des Rands. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Liest oder setzt den Zellenrandtyp. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Liest und setzt die Designfarbe des Rands. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
            workbook.Worksheets.Add();

            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Cell cell = worksheet.Cells["A1"];

            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Hello World");

            // Abrufen des Zellenstils
            Style style = cell.GetStyle();

            // Festlegen des Linienstils des oberen Rahmens
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Festlegen des Linienstils des unteren Rahmens
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Festlegen des Linienstils des linken Rahmens
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Festlegen des Linienstils des rechten Rahmens
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Den Stil auf die Zelle anwenden
            cell.SetStyle(style);

            // Die Excel-Datei speichern
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


