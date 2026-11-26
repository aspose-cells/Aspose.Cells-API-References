---
title: "Comment.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa la altura del comentario en unidades de píxeles"
type: docs
url: /es/net/aspose.cells/comment/height/
---
## Comment.Height property

Representa la altura del comentario, en unidades de píxeles.

```csharp
public int Height { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            // Demostrar la propiedad Height
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


