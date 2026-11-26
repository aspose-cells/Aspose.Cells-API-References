---
title: "Shape.Paths"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene las rutas de una forma geométrica personalizada"
type: docs
url: /es/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Obtiene las rutas de una forma geométrica personalizada.

```csharp
public ShapePathCollection Paths { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma personalizada (rectángulo) con parámetros correctos
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Verifica si la forma tiene rutas de geometría personalizada
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Agrega una nueva ruta a la geometría de la forma
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### Ver también

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


