---
title: "Klasse ThreadedComment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ThreadedComment Klasse. Repräsentiert den Threaded Comment"
type: docs
url: /de/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Stellt den Threaded‑Kommentar dar.

```csharp
public class ThreadedComment
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Liefert den Autor des Kommentars. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Liefert den Spaltenindex des Kommentars. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Liefert und setzt die Erstellungszeit dieses Threaded Comments. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Liefert und setzt den Text des Kommentars. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Liefert den Zeilenindex des Kommentars. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Autoren zum Arbeitsbuch hinzu
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Hole Autorenreferenzen
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Füge einen Threaded Comment dem Kommentar hinzu
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Zusätzliche Eigenschaften festlegen
            threadedComment.Notes = "Additional notes";
            
            // Füge eine Antwort zum Threaded Comment hinzu
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Speichere die Arbeitsmappe
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


