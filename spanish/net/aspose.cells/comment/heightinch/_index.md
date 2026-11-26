---
title: "Comment.HeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa la altura del comentario en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Representa la altura del comentario, en unidades de pulgadas.

```csharp
public double HeightInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HeightInch = 1.5;
            Console.WriteLine("Comment height set to: " + comment.HeightInch + " inches");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


