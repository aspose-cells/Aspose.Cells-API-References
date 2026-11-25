---
title: "CommentCollection.GetThreadedComments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CommentCollection. Ottiene i commenti in thread per indice di riga e colonna"
type: docs
url: /it/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Restituisce i commenti in thread per indice di riga e colonna.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Esempi

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Vedi anche

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Restituisce i commenti in thread per nome della cella.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Il nome della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un autore di commento in thread e ottieni l'autore per indice
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Aggiungi un commento in thread alla cella B2
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // Ottieni tutti i commenti in thread per la cella B2
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Visualizza i commenti in thread
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### Vedi anche

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


