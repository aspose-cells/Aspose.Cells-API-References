---
title: "ThreadedComment.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedComment-Eigenschaft. Gibt den Spaltenindex des Kommentars zurück"
type: docs
url: /de/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Liefert den Spaltenindex des Kommentars.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Erstellen Sie zuerst einen ThreadedComment-Autor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // Füge einen ThreadedComment zu Zelle A1 (Zeile 0, Spalte 0) hinzu
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // Den ersten ThreadedComment abrufen
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Zeigen Sie den Wert der Column-Eigenschaft an (schreibgeschützt)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Überprüfen Sie, ob der Spaltenindex mit der Position des Kommentars übereinstimmt
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


