---
title: "Comment.WidthCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa el ancho del comentario en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/comment/widthcm/
---
## Comment.WidthCM property

Representa el ancho del comentario, en unidades de centímetros.

```csharp
public double WidthCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            comment.WidthCM = 5.0;

            Console.WriteLine($"Comment width set to: {comment.WidthCM} cm");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


