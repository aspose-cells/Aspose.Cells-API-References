---
title: "Comment.WidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa el ancho del comentario en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

Representa el ancho del comentario, en unidades de pulgadas.

```csharp
public double WidthInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            comment.WidthInch = 1.5;
            
            Console.WriteLine("Comment width set to: " + comment.WidthInch + " inches");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


