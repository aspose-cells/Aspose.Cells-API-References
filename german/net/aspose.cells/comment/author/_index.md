---
title: "Comment.Author"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Ruft den Namen des ursprünglichen Kommentarautors ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells/comment/author/
---
## Comment.Author property

Liest und setzt den Namen des ursprünglichen Kommentarautors

```csharp
public string Author { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Setze den Kommentarautor und die Notiz
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Zeige den Kommentarautor an
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


