---
title: "ShapeCollection.Ungroup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Desagrupa los elementos de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Desagrupa los elementos de la forma.

```csharp
public void Ungroup(GroupShape group)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| grupo | GroupShape | La forma de grupo. |

### Observaciones

Si la forma de grupo está agrupada por otra forma de grupo, no se hará nada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUngroupWithGroupShapeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar primera forma rectangular
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Agregar segunda forma rectangular
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Crear matriz de formas para agrupar
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Agrupar las formas
            GroupShape groupShape = shapes.Group(shapesArr);

            // Desagrupar la forma de grupo
            shapes.Ungroup(groupShape);
        }
    }
}
```

### Ver también

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


