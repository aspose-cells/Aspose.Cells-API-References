---
title: "ShapeCollection.Group"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrupa las formas"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Agrupa las formas.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| groupItems | Shape[] | los elementos del grupo. |

### Valor de retorno

Devuelve la forma del grupo.

### Observaciones

La forma en groupItems no debe estar agrupada. La forma debe estar en esta colección Shapes.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodGroupWithShapeArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar primera forma rectangular
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Agregar segunda forma rectangular
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Crear una matriz con las formas a agrupar
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Agrupar las formas
            GroupShape groupShape = shapes.Group(shapesArr);

            // Guarda el libro de trabajo
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


