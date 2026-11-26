---
title: "Comment.TextHorizontalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene y establece el tipo de alineación horizontal del texto del comentario"
type: docs
url: /es/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

Obtiene y establece el tipo de alineación horizontal del texto del comentario.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Establecer la alineación horizontal inicial a Fill
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // Cambiar la alineación a Center si era Fill
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
            }
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


