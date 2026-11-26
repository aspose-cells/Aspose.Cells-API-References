---
title: "Shape.Geometry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene la geometría"
type: docs
url: /es/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Obtiene la geometría

```csharp
public Geometry Geometry { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGeometryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Verificar propiedades de la geometría
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Agregar un punto de ajuste (demostrando la modificación de la geometría)
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


