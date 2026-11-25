---
title: "CommentCollection.AddThreadedComment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CommentCollection. Aggiunge un commento in thread"
type: docs
url: /it/net/aspose.cells/commentcollection/addthreadedcomment/
---
## AddThreadedComment(int, int, string, ThreadedCommentAuthor) {#addthreadedcomment}

Aggiunge un commento a thread.

```csharp
public int AddThreadedComment(int row, int column, string text, ThreadedCommentAuthor author)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga della cella. |
| colonna | Int32 | Indice di colonna della cella. |
| testo | String | Il testo del commento |
| autore | ThreadedCommentAuthor | L'utente di questo commento in thread. |

### Valore di ritorno

[`ThreadedComment`](../../threadedcomment/) object index.

### Esempi

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

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddThreadedComment(string, string, ThreadedCommentAuthor) {#addthreadedcomment_1}

Aggiunge un commento a thread.

```csharp
public int AddThreadedComment(string cellName, string text, ThreadedCommentAuthor author)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Il nome della cella. |
| testo | String | Il testo del commento |
| autore | ThreadedCommentAuthor | L'utente di questo commento in thread. |

### Valore di ritorno

[`ThreadedComment`](../../threadedcomment/) object index.

### Esempi

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

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


