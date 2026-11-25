---
title: "Classe Comment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Comment class. Incapsula l'oggetto che rappresenta un commento di cella"
type: docs
url: /it/net/aspose.cells/comment/
---
## Comment class

Incapsula l'oggetto che rappresenta un commento di cella.

```csharp
public class Comment
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Ottiene e imposta il Nome dell'autore originale del commento |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Indica se la dimensione del commento viene regolata automaticamente in base al suo contenuto. Nota: in alcuni casi speciali (come l'ambiente Mac), questa impostazione potrebbe non avere effetto. Se questa impostazione non ha effetto, si prega di sostituirla con FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Ottiene l'indice di colonna del commento. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Ottieni un oggetto Shape che rappresenta la forma allegata al commento specificato. |
| [Font](../../aspose.cells/comment/font/) { get; } | Ottiene il carattere del commento. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Rappresenta l'Altezza del commento, in unità di pixel. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Rappresenta l'altezza del commento, in unità di centimetri. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Rappresenta l'altezza del commento, in unità di pollici. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Ottiene e imposta la stringa HTML che contiene dati e alcuni formati in questo commento. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Indica se questo commento è un commento a thread. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Rappresenta se il commento è visibile o meno. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Rappresenta il contenuto del commento. |
| [Row](../../aspose.cells/comment/row/) { get; } | Ottiene l'indice di riga del commento. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Ottiene e imposta il tipo di allineamento orizzontale del testo del commento. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Ottiene e imposta il tipo di orientamento del testo del commento. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Ottiene e imposta il tipo di allineamento verticale del testo del commento. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Ottiene l'elenco dei commenti a thread; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Rappresenta la larghezza del commento, in unità di pixel. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Rappresenta la larghezza del commento, in unità di centimetri. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Rappresenta la larghezza del commento, in unità di pollici. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo del commento. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Formatta alcuni caratteri con l'impostazione del font. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo del commento. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Accedi alla raccolta dei commenti del foglio di lavoro
            CommentCollection comments = worksheet.Comments;

            // Aggiungi un commento alla cella A1
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

            // Accedi alla forma del commento
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // Aggiungi un commento alla cella B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Salva la cartella di lavoro
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


