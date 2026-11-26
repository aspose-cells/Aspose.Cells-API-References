---
title: "ShapeCollection.Remove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Elimina la forma"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Elimina la forma.

```csharp
public void Remove(Shape shape)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| forma | Forma |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveWithShapeDemo
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

            // Obtener la primera forma por nombre o índice
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Eliminar la forma de la colección
                shapes.Remove(shapeToRemove);
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


