---
title: "Comment.HeightCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa la altura del comentario en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Representa la altura del comentario, en unidades de centímetros.

```csharp
public double HeightCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Establecer texto del comentario
            comment.Note = "Sample comment";
            
            // Establecer la altura del comentario en centímetros
            comment.HeightCM = 1.5;
            
            // Guarda el libro de trabajo
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


