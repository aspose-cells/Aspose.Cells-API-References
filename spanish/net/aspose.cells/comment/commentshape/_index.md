---
title: "Comment.CommentShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtenga un objeto Shape que representa la forma adjunta al comentario especificado"
type: docs
url: /es/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

Obtén un objeto Shape que representa la forma adjunta al comentario especificado.

```csharp
public CommentShape CommentShape { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentPropertyCommentShapeDemo
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

            // Obtener el CommentShape y modificar sus propiedades
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // Mostrar las dimensiones de la forma
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### Ver también

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


