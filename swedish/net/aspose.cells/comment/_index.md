---
title: Comment
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar en cellkommentar.
type: docs
weight: 1080
url: /sv/net/aspose.cells/comment/
---
## Comment class

Kapslar in objektet som representerar en cellkommentar.

```csharp
public class Comment
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells/comment/author) { get; set; } | Hämtar och ställer in Namn på den ursprungliga kommentaren author |
| [AutoSize](../../aspose.cells/comment/autosize) { get; set; } | Indikerar om storleken på kommentaren justeras automatiskt enligt dess innehåll. |
| [Column](../../aspose.cells/comment/column) { get; } | Hämtar kolumnindex för kommentaren. |
| [CommentShape](../../aspose.cells/comment/commentshape) { get; } | Hämta ett Shape-objekt som representerar formen kopplad till den angivna kommentaren. |
| [Font](../../aspose.cells/comment/font) { get; } | Får typsnittet för kommentar. |
| [Height](../../aspose.cells/comment/height) { get; set; } | Representerar höjden på kommentaren, i enhet pixlar. |
| [HeightCM](../../aspose.cells/comment/heightcm) { get; set; } | Representerar höjden på kommentaren, i centimeterenhet. |
| [HeightInch](../../aspose.cells/comment/heightinch) { get; set; } | Representerar höjden på kommentaren, i enhet av tum. |
| [HtmlNote](../../aspose.cells/comment/htmlnote) { get; set; } | Hämtar och ställer in html-strängen som innehåller data och vissa format i denna kommentar. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment) { get; } | Indikerar om denna kommentar är en trådad kommentar. |
| [IsVisible](../../aspose.cells/comment/isvisible) { get; set; } | Representerar om kommentaren är synlig eller inte. |
| [Note](../../aspose.cells/comment/note) { get; set; } | Representerar innehållet i kommentaren. |
| [Row](../../aspose.cells/comment/row) { get; } | Hämtar radindex för kommentaren. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment) { get; set; } | Hämtar och ställer in textens horisontella justering av kommentaren. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype) { get; set; } | Hämtar och ställer in textorienteringstypen för kommentaren. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment) { get; set; } | Hämtar och ställer in den vertikala textjusteringstypen för kommentaren. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments) { get; } | Hämtar listan med trådade kommentarer; |
| [Width](../../aspose.cells/comment/width) { get; set; } | Representerar bredden på kommentaren, i enhet pixlar. |
| [WidthCM](../../aspose.cells/comment/widthcm) { get; set; } | Representerar bredden på kommentaren, i centimeterenhet. |
| [WidthInch](../../aspose.cells/comment/widthinch) { get; set; } | Representerar bredden på kommentaren, i enhet av tum. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters)(int, int) | Returnerar ett teckenobjekt som representerar ett antal tecken i kommentarstexten. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters)(int, int, Font, StyleFlag) | Formatera några tecken med teckensnittsinställningen. |
| [GetCharacters](../../aspose.cells/comment/getcharacters)() | Returnerar alla teckenobjekt som representerar ett antal tecken i kommentarstexten. |

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();
CommentCollection comments = workbook.Worksheets[0].Comments;

//Lägg till kommentar i cell A1
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";

//Lägg till kommentar i cell B2
comments.Add("B2");
Comment comment2 = comments["B2"];
comment2.Note = "Second note.";

//gör dina affärer

//Spara excel-filen.
workbook.Save("exmaple.xlsx");

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim comments as CommentCollection = workbook.Worksheets(0).Comments
 
'Lägg till kommentar i cell A1
Dim commentIndex1 as Integer = comments.Add(0, 0)
Dim comment1 as Comment = comments(commentIndex1)
comment1.Note = "First note."
comment1.Font.Name = "Times New Roman"

'Lägg till kommentar i cell B2
comments.Add("B2")
Dim comment2 As Comment = comments("B2")
comment2.Note = "Second note."
 
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
