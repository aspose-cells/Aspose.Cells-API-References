---
title: "ShapeCollection.DeleteShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Eliminar una forma. Si la forma está en el grupo o es una forma de comentario, no se eliminará"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Elimina una forma. Si la forma está en el grupo o es una forma de comentario, no se eliminará.

```csharp
public void DeleteShape(Shape shape)
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
    public class ShapeCollectionMethodDeleteShapeWithShapeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar primera forma rectangular
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Agregar segunda forma rectangular
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Eliminar la primera forma
            shapes.DeleteShape(firstShape);

            // Guarda el libro de trabajo
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


