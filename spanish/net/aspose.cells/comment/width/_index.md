---
title: "Comment.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa el ancho del comentario en unidades de píxeles"
type: docs
url: /es/net/aspose.cells/comment/width/
---
## Comment.Width property

Representa el ancho del comentario, en unidades de píxeles.

```csharp
public int Width { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Establecer propiedades del comentario
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Guarda el libro de trabajo
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


