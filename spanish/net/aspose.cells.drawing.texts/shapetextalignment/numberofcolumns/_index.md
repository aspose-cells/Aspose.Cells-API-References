---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene y establece el número de columnas de texto en el rectángulo delimitador"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Obtiene y establece el número de columnas de texto en el rectángulo delimitador.

```csharp
public int NumberOfColumns { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Establecer texto para la forma
            shape.Text = "This is sample text\nin multiple columns";
            
            // Acceder a la alineación de texto y establecer el número de columnas
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar la propiedad
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


