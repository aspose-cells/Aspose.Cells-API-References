---
title: "CommentCollection.AddThreadedComment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CommentCollection. Agrega un comentario en hilo"
type: docs
url: /es/net/aspose.cells/commentcollection/addthreadedcomment/
---
## AddThreadedComment(int, int, string, ThreadedCommentAuthor) {#addthreadedcomment}

Agrega un comentario en hilo.

```csharp
public int AddThreadedComment(int row, int column, string text, ThreadedCommentAuthor author)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda. |
| columna | Int32 | Índice de columna de la celda. |
| texto | String | El texto del comentario |
| autor | ThreadedCommentAuthor | El usuario de este comentario en hilo. |

### Valor de retorno

[`ThreadedComment`](../../threadedcomment/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddThreadedCommentWithInt32Int32StringThreadedCommenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CommentCollection comments = worksheet.Comments;
            
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demoUser", "testProvider");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            comments.AddThreadedComment(1, 1, "This is a threaded comment demo.", author);
            
            var threadedComments = comments.GetThreadedComments(1, 1);
            foreach (var comment in threadedComments)
            {
                Console.WriteLine(comment.Notes);
            }

            workbook.Save("ThreadedCommentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddThreadedComment(string, string, ThreadedCommentAuthor) {#addthreadedcomment_1}

Agrega un comentario en hilo.

```csharp
public int AddThreadedComment(string cellName, string text, ThreadedCommentAuthor author)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | El nombre de la celda. |
| texto | String | El texto del comentario |
| autor | ThreadedCommentAuthor | El usuario de este comentario en hilo. |

### Valor de retorno

[`ThreadedComment`](../../threadedcomment/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddThreadedCommentWithStringStringThreadedCommentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            CommentCollection comments = worksheet.Comments;
            comments.AddThreadedComment("B3", "Initial comment text", author);
            comments.AddThreadedComment("C5", "Follow-up comment", author);
            
            workbook.Save("ThreadedCommentsOutput.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


