---
title: "Comment.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene la fuente del comentario"
type: docs
url: /es/net/aspose.cells/comment/font/
---
## Comment.Font property

Obtiene la fuente del comentario.

```csharp
public Font Font { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Acceder y modificar las propiedades de fuente del comentario
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Guarda el libro de trabajo
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


