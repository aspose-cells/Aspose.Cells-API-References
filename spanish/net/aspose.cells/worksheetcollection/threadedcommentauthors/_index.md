---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene la lista de autores de comentarios en hilo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

Obtiene la lista de autores de comentarios en hilo.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un autor de comentario en hilo
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // Obtener el autor que acabamos de agregar
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Agregar comentarios en hilo a la celda C2
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // Guarda el libro de trabajo
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // Obtener la celda donde queremos agregar el comentario
            Cell cell = worksheet.Cells[cellName];
            
            // Agregar un comentario en hilo (devuelve void, no ThreadedComment)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


