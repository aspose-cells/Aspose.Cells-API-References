---
title: "CommentCollection.GetThreadedComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CommentCollection. Obtiene los comentarios en hilo por índice de fila y columna"
type: docs
url: /es/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Obtiene los comentarios en hilo por índice de fila y columna.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Ejemplos

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Ver también

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Obtiene los comentarios en hilo por nombre de celda.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | El nombre de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un autor de comentario en hilo y obtener el autor por índice
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Agregar un comentario en hilo a la celda B2
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // Obtener todos los comentarios en hilo para la celda B2
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Mostrar los comentarios en hilo
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### Ver también

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


