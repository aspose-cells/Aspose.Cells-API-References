---
title: "ThreadedComment.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedComment-Eigenschaft. Gibt den Zeilenindex des Kommentars zurück"
type: docs
url: /de/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Liefert den Zeilenindex des Kommentars.

```csharp
public int Row { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Erstellen Sie einen ThreadedComment-Autor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // Fügen Sie einen ThreadedComment zu Zelle B2 (Zeile 1, Spalte 1) hinzu
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // Den ersten ThreadedComment abrufen
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Zeigen Sie den Wert der Row-Eigenschaft an (schreibgeschützt)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Überprüfen Sie, ob der Zeilenindex mit der Position des Kommentars übereinstimmt
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ThreadedCommentRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


