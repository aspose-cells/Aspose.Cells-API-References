---
title: "Klasse TextParagraph"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextParagraph Klasse. Stellt die Textelementabsatzeinstellung dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Stellt die Einstellung des Textabsatzes dar.

```csharp
public class TextParagraph : FontSetting
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Liest und setzt den horizontalen Ausrichtungstyp des Textes im Absatz. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Liest das Aufzählungszeichen. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Liest alle Textabschnitte in diesem Absatz. Wenn dieser Absatz leer ist, wird der Absatz selbst zurückgegeben. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Liest und setzt die Standardgröße für ein Tabulatorzeichen in diesem Absatz. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Gibt die Einzugsgröße an, die auf die erste Textzeile im Absatz angewendet wird. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Gibt die Schriftart dieses Objekts zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert sind. Dies betrifft die vertikale Anordnung der Zeichen in Bezug auf die Grundlinien. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Gibt an, ob ein ostasiatisches Wort ohne Hinzufügen eines Bindestrichs am Ende in zwei Teile getrennt und in die nächste Zeile umbrochen werden kann. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Gibt an, ob ein lateinisches Wort ohne Hinzufügen eines Bindestrichs am Ende in zwei Teile getrennt und in die nächste Zeile umbrochen werden kann. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Gibt den linken Rand des Absatzes an. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Liest die Länge der Zeichen. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Liest und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Liest und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Gibt den rechten Rand des Absatzes an. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Liest und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden sein wird. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Liest und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden sein wird. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Liest und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden sein wird. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Liest und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden sein wird. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Liest den Startindex der Zeichen. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Liest die Tabulatorliste. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Gibt die Textoptionen zurück. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Ermittelt den Typ des Textknotens. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Setzt den vordefinierten WordArt-Stil. (Geerbt von [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Setzt den Textinhalt mit mehreren Absätzen
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Zugriff auf Textabsätze und deren Bearbeitung
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Setzt Absatz-Eigenschaften
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


