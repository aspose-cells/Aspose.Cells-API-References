---
title: "Comment.TextVerticalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene y establece el tipo de alineación vertical del texto del comentario"
type: docs
url: /es/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Obtiene y establece el tipo de alineación vertical del texto del comentario.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Establecer la alineación vertical a Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Cambiar la alineación vertical a Center si era Fill
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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


