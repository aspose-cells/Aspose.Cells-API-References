---
title: "Comment.TextOrientationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene y establece el tipo de orientación del texto del comentario"
type: docs
url: /es/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Obtiene y establece el tipo de orientación del texto del comentario.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Establecer la orientación inicial a NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Cambiar la orientación a TopToBottom si actualmente es NoRotation
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Guarda el libro de trabajo
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


