---
title: "Comment.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa si el comentario es visible o no"
type: docs
url: /es/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Representa si el comentario es visible o no.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Establece el comentario como visible
            comment.IsVisible = true;

            // Comprueba si el comentario es visible
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Guarda el libro de trabajo
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


