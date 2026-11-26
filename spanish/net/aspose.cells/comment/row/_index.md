---
title: "Comment.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene el índice de fila del comentario"
type: docs
url: /es/net/aspose.cells/comment/row/
---
## Comment.Row property

Obtiene el índice de fila del comentario.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Obtener y mostrar el índice de fila de la celda comentada
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // Agregar otro comentario a la celda B3
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // Mostrar el índice de fila del segundo comentario
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


