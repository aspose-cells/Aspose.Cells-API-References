---
title: "Shape.HeightInShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre en unidades de 1/4000 de la altura de la forma padre"
type: docs
url: /es/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Representa el desplazamiento vertical de la forma desde el borde superior de la forma padre, en unidades de 1/4000 de la altura de la forma padre..

```csharp
public int HeightInShape { get; set; }
```

### Observaciones

Solo se aplica cuando esta forma está en el grupo o gráfico.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar formas primero con todos los parámetros requeridos
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Agrupar las formas
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Establecer la altura del rectángulo relativa a la forma de grupo padre (1/4000 de la altura del padre)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Guarda el libro de trabajo
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


