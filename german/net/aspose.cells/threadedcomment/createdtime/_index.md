---
title: "ThreadedComment.CreatedTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedComment-Eigenschaft. Gibt die Erstellungszeit dieses ThreadedComment zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Liefert und setzt die Erstellungszeit dieses Threaded Comments.

```csharp
public DateTime CreatedTime { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen ThreadedComment-Autor
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Threaded Comment hinzufügen
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Demonstrieren Sie die CreatedTime-Eigenschaft
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


