---
title: "Klasse Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Column class. Stellt eine einzelne Spalte in einem Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells/column/
---
## Column class

Stellt eine einzelne Spalte in einem Arbeitsblatt dar.

```csharp
public class Column
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Ermittelt die Gruppenebene der Spalte. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Gibt an, ob diese Spalte benutzerdefinierte Formatierungseinstellungen hat (anders als die standardmäßige, vom Arbeitsbuch geerbte). |
| [Index](../../aspose.cells/column/index/) { get; } | Ermittelt den Index dieser Spalte. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | ob die Spalte zusammengeklappt ist |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Gibt an, ob die Spalte ausgeblendet ist. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Ermittelt den Stil dieser Spalte. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Ermittelt und legt die Spaltenbreite in Zeichen als Einheit fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Wendet Formate für eine ganze Spalte an. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Ermittelt den Stil dieser Spalte. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Legt den Stil dieser Spalte fest. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ermitteln der Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            // Neuen Stil zur Arbeitsmappe hinzufügen
            Style style = workbook.CreateStyle();

            // Setzt die Hintergrundfarbe auf Blau
            style.BackgroundColor = Color.Blue;

            // Setzt die Vordergrundfarbe auf Rot
            style.ForegroundColor = Color.Red;

            // Setzt das Hintergrundmuster
            style.Pattern = BackgroundType.DiagonalStripe;

            // Neues Stil-Flag
            StyleFlag styleFlag = new StyleFlag();

            // Alle Stile festlegen
            styleFlag.All = true;

            // Erste Spalte abrufen
            Column column = worksheet.Cells.Columns[0];

            // Stil auf die erste Spalte anwenden
            column.ApplyStyle(style, styleFlag);

            // Zusätzliche Eigenschaften festlegen
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Die Excel-Datei speichern
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


