---
title: "Klasse StyleFlag"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.StyleFlag Klasse. Stellt Flags dar, die angewendete Formatierungseigenschaften anzeigen."
type: docs
url: /de/net/aspose.cells/styleflag/
---
## StyleFlag class

Stellt Flags dar, die angewendete Formatierungseigenschaften anzeigen.

```csharp
public class StyleFlag
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [StyleFlag](styleflag/)() | Konstruiert ein Objekt, bei dem alle Flags auf false gesetzt sind. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Ausrichtungseinstellung wird angewendet. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Alle Eigenschaften werden angewendet. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Alle Rahmen-Einstellungen werden angewendet. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Die Einstellungen für den unteren Rand werden angewendet. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Die Einstellung für die Zellen-Schattierung wird angewendet. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Die Einstellungen für den diagonalen Abwärtsrahmen werden angewendet. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Die Einstellungen für den diagonalen Aufwärtsrahmen werden angewendet. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Die Schriftarteinstellungen werden angewendet. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Die Einstellung für fette Schrift wird angewendet. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Die Einstellung für die Schriftfarbe wird angewendet. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Die Einstellung für kursiven Text wird angewendet. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Die Einstellung für den Schriftartnamen wird angewendet. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Die Einstellung für das Schriftskript wird angewendet. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Die Einstellung für die Schriftgröße wird angewendet. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Die Einstellung für durchgestrichene Schrift wird angewendet. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Die Einstellung für unterstrichene Schrift wird angewendet. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Die Einstellung zum Ausblenden von Formeln wird angewendet. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Die Einstellung für die horizontale Ausrichtung wird angewendet. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Die Einstellung für die Einzugsebene wird angewendet. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Die Einstellungen für den linken Rand werden angewendet. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Die gesperrte Einstellung wird angewendet. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Die Einstellung für das Zahlenformat wird angewendet. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Die Einstellung zum Ausblenden von Formeln wird angewendet. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Die Einstellungen für den rechten Rand werden angewendet. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Die Rotationseinstellung wird angewendet. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Die Einstellung 'Verkleinern, um anzupassen' wird angewendet. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Die Einstellung für die Textausrichtung wird angewendet. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Die Einstellungen für den oberen Rand werden angewendet. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Die Einstellung für die vertikale Ausrichtung wird angewendet. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Die Einstellung zum Zeilenumbruch wird angewendet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Ein neues Style-Objekt erstellen
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Ein neues StyleFlag-Objekt erstellen
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Den Stil auf einen Zellbereich anwenden
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


