---
title: "Comment.Author"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene e imposta il nome dell'autore originale del commento"
type: docs
url: /it/net/aspose.cells/comment/author/
---
## Comment.Author property

Ottiene e imposta il Nome dell'autore originale del commento

```csharp
public string Author { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Imposta l'autore del commento e la nota
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Visualizza l'autore del commento
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


