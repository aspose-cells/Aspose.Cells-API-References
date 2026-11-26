---
title: "Shape.IsDecorative"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Indica si el objeto es decorativo"
type: docs
url: /es/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Indica si el objeto es decorativo.

```csharp
public bool IsDecorative { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // Establecer el shape como decorativo
            shape.IsDecorative = true;
            
            // Guarda el libro de trabajo
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recargar el libro de trabajo para verificar la propiedad
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Mostrar el resultado
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


