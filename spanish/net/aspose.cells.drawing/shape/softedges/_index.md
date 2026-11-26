---
title: "Shape.SoftEdges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene y establece el radio de desenfoque que se aplicará a los bordes en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Obtiene y establece el radio de desenfoque a aplicar en los bordes, en unidades de puntos.

```csharp
public double SoftEdges { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Establece el efecto de bordes suaves con un radio de 5 puntos (0.5d = 5 puntos)
            shape.SoftEdges = 0.5d;

            // Guarda el libro de trabajo
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


