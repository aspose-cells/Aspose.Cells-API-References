---
title: "Klasse Comment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Comment-Klasse. Kapselt das Objekt, das einen Zellkommentar darstellt"
type: docs
url: /de/net/aspose.cells/comment/
---
## Comment class

Kapselt das Objekt, das einen Zellenkommentar darstellt.

```csharp
public class Comment
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Liest und setzt den Namen des ursprünglichen Kommentarautors |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Gibt an, ob die Größe des Kommentars automatisch an seinen Inhalt angepasst wird. Hinweis: In einigen Sonderfällen (z. B. in einer Mac-Umgebung) kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Liefert den Spaltenindex des Kommentars. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Erhalte ein Shape-Objekt, das die dem angegebenen Kommentar zugefügte Form darstellt. |
| [Font](../../aspose.cells/comment/font/) { get; } | Liest die Schriftart des Kommentars. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Stellt die Höhe des Kommentars in Pixeln dar. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Stellt die Höhe des Kommentars in Zentimetern dar. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Stellt die Höhe des Kommentars in Zoll dar. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Liest und setzt die HTML-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Gibt an, ob dieser Kommentar ein Threaded Comment ist. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Stellt dar, ob der Kommentar sichtbar ist oder nicht. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Stellt den Inhalt des Kommentars dar. |
| [Row](../../aspose.cells/comment/row/) { get; } | Liefert den Zeilenindex des Kommentars. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Liest und setzt den horizontalen Ausrichtungstyp des Textes im Kommentar. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Liest und setzt den Orientierungstyp des Textes im Kommentar. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Liest und setzt den vertikalen Ausrichtungstyp des Textes im Kommentar. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Liest die Liste der Threaded Comments; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Stellt die Breite des Kommentars in Pixeln dar. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Stellt die Breite des Kommentars in Zentimetern dar. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Stellt die Breite des Kommentars in Zoll dar. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Kommentartext darstellt. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Formatiere einige Zeichen mit den Schriftarteinstellungen. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Kommentartext darstellen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CommentDemo
    {
        public static void CommentExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            // Greife auf die Kommentare-Sammlung des Arbeitsblatts zu
            CommentCollection comments = worksheet.Comments;

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            comment1.Font.Size = 12;
            comment1.Font.Color = System.Drawing.Color.Red;
            comment1.Author = "Carl.Yang";
            comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            comment1.IsVisible = true;
            comment1.TextOrientationType = TextOrientationType.TopToBottom;
            comment1.TextHorizontalAlignment = TextAlignmentType.Center;
            comment1.TextVerticalAlignment = TextAlignmentType.Center;
            comment1.AutoSize = true;
            comment1.HeightCM = 1.0;
            comment1.WidthCM = 1.0;
            comment1.Width = 10;
            comment1.Height = 10;
            comment1.WidthInch = 1.0;
            comment1.HeightInch = 1.0;

            // Greife auf die Form des Kommentars zu
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // Füge einen Kommentar zur Zelle B2 hinzu
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Speichere die Arbeitsmappe
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


