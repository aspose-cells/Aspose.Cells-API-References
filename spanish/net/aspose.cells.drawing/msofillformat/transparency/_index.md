---
title: "MsoFillFormat.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFillFormat. Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Establece propiedades de formato de relleno incluyendo la transparencia
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Establece la transparencia (0.0 = totalmente opaco, 1.0 = totalmente transparente)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Guarda el libro de trabajo
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Carga el libro de trabajo guardado para verificar la transparencia
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Muestra el valor de transparencia para demostrar que se guardó y cargó correctamente
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### Ver también

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


