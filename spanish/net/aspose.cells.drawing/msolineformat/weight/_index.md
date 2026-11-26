---
title: "MsoLineFormat.Weight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormat. Devuelve o establece el grosor de la línea en unidades de pt"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Devuelve o establece el grosor de la línea, en unidades de pt.

```csharp
public double Weight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
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
            
            // Establecer el texto del comentario
            comment.Note = "Sample comment";
            
            // Acceder al formato de línea de la forma de comentario y establecer el grosor
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar que el grosor se haya establecido correctamente
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### Ver también

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


