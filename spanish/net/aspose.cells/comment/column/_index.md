---
title: "Comment.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene el índice de columna del comentario"
type: docs
url: /es/net/aspose.cells/comment/column/
---
## Comment.Column property

Obtiene el índice de columna del comentario.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda B5 (índice de columna 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Establecer texto del comentario
            comment.Note = "This is a sample comment";

            // Demostrar el uso de la propiedad Column
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Verificar que el índice de columna coincida con donde lo colocamos
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


