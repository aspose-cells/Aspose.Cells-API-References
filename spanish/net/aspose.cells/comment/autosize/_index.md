---
title: "Comment.AutoSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Indica si el tamaño del comentario se ajusta automáticamente según su contenido. Nota: en algunos casos especiales, como en entornos Mac, esta configuración puede no tener efecto. Si esta configuración no tiene efecto, por favor reemplácela por FitToTextSize"
type: docs
url: /es/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Indica si el tamaño del comentario se ajusta automáticamente según su contenido. Nota: En algunos casos especiales (como el entorno Mac), esta configuración puede no tener efecto. Si esta configuración no tiene efecto, por favor reemplácela con FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // Establecer AutoSize a true
            comment.AutoSize = true;

            // Guarda el libro de trabajo
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


