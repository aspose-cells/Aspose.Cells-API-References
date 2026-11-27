---
title: "Klass Kommentar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Comment-klass. Inkapslar objektet som representerar en cellkommentar"
type: docs
url: /sv/net/aspose.cells/comment/
---
## Comment class

Inkapslar objektet som representerar en cellkommentar.

```csharp
public class Comment
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Hämtar och anger namn på den ursprungliga kommentarsförfattaren |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Anger om kommentarsstorleken justeras automatiskt enligt dess innehåll. Obs: I vissa speciella fall (t.ex. Mac-miljö) kan denna inställning vara utan effekt. Om den inte har någon effekt, ersätt den med FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Hämtar kolumnindexet för kommentaren. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Hämta ett Shape-objekt som representerar formen som är bifogad till den angivna kommentaren. |
| [Font](../../aspose.cells/comment/font/) { get; } | Hämtar kommentarsfonten. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Representerar kommentarsens höjd i pixlar. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Representerar kommentarsens höjd i centimeter. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Representerar kommentarsens höjd i tum. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Hämtar och anger html-strängen som innehåller data och vissa format i denna kommentar. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Anger om denna kommentar är en trådad kommentar. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Representerar om kommentaren är synlig eller inte. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Representerar kommentarinnehållet. |
| [Row](../../aspose.cells/comment/row/) { get; } | Hämtar radindexet för kommentaren. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Hämtar och anger den horisontella justeringstypen för kommentaren. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Hämtar och anger textorienteringstypen för kommentaren. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Hämtar och anger den vertikala justeringstypen för kommentaren. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Hämtar listan över trådade kommentarer; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Representerar bredden på kommentaren, i enhet pixlar. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Representerar bredden på kommentaren, i enhet centimeter. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Representerar bredden på kommentaren, i enhet tum. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Returnerar ett Characters-objekt som representerar ett intervall av tecken i kommentartexten. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Formatera vissa tecken med teckensnittsinställningen. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Returnerar alla Characters-objekt som representerar ett intervall av tecken i kommentartexten. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Åtkomst till kommentarssamlingen i kalkylbladet
            CommentCollection comments = worksheet.Comments;

            // Lägg till en kommentar till cell A1
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

            // Åtkomst till kommentarsformen
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // Lägg till en kommentar i cell B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Spara arbetsboken
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


