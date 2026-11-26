---
title: "Shape.ThreeDFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el formato 3D de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

Obtiene y establece el formato 3D de la forma.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Acceder y modificar las propiedades del formato 3D
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


