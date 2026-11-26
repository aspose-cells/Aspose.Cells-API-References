---
title: "Comment.Author"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene y establece el nombre del autor original del comentario"
type: docs
url: /es/net/aspose.cells/comment/author/
---
## Comment.Author property

Obtiene y establece el Nombre del autor original del comentario

```csharp
public string Author { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Establecer el autor y la nota del comentario
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Mostrar el autor del comentario
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


