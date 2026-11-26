---
title: "Comment.Note"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Representa el contenido del comentario"
type: docs
url: /es/net/aspose.cells/comment/note/
---
## Comment.Note property

Representa el contenido del comentario.

```csharp
public string Note { get; set; }
```

### Observaciones

Si este es un comentario en hilo, la nota no se puede cambiar, de lo contrario MS Excel no podría procesarlo como un comentario en hilo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Establecer la nota del comentario
            comment1.Note = "First note.";
            
            // Verificar que la nota se haya establecido
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


