---
title: "Comment.IsThreadedComment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Indica se questo commento è un commento a thread"
type: docs
url: /it/net/aspose.cells/comment/isthreadedcomment/
---
## Comment.IsThreadedComment property

Indica se questo commento è un commento a thread.

```csharp
public bool IsThreadedComment { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsThreadedCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento normale
            Comment regularComment = worksheet.Comments[worksheet.Comments.Add("A1")];
            regularComment.Note = "This is a regular comment";
            regularComment.Author = "User1";

            // Aggiungi un commento a thread (supponendo che l'API supporti l'aggiunta di commenti a thread)
            Comment threadedComment = worksheet.Comments[worksheet.Comments.Add("B1")];
            threadedComment.Note = "This is a threaded comment";
            threadedComment.Author = "User2";

            // Verifica i tipi di commento
            Console.WriteLine("Comment at A1 is threaded: " + regularComment.IsThreadedComment);
            Console.WriteLine("Comment at B1 is threaded: " + threadedComment.IsThreadedComment);

            // Elabora i commenti in base al loro tipo
            foreach (Comment comment in worksheet.Comments)
            {
                if (comment.IsThreadedComment)
                {
                    Console.WriteLine($"Threaded comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                    Console.WriteLine($"Author: {comment.Author}, Note: {comment.Note}");
                }
                else
                {
                    Console.WriteLine($"Regular comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                }
            }
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


