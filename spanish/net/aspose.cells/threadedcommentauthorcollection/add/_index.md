---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ThreadedCommentAuthorCollection. Añade una persona de comentario en hilo"
type: docs
url: /es/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Agrega una persona de comentario en hilo.

```csharp
public int Add(string name, string userId, string providerId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la persona. |
| userId | String |  |
| providerId | String | El id del proveedor |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un autor de comentario en hilo
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Obtener el autor añadido
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Agregar comentarios en hilo usando el autor
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Guarda el libro de trabajo
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### Ver también

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


