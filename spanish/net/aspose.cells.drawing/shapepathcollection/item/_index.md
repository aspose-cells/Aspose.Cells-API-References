---
title: "ShapePathCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathCollection. Obtiene una ruta de creación"
type: docs
url: /es/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Obtiene una ruta de creación.

```csharp
public ShapePath this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

Devuelve el objeto [`ShapePath`](../../shapepath/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma personalizada (forma no primitiva) con los parámetros correctos
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // Accede a la ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Agregar una nueva ruta
            int pathIndex = shapePaths.Add();

            // Acceder a la ruta usando la propiedad Item
            ShapePath newPath = shapePaths[pathIndex];

            // Información de salida
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Guarda el libro de trabajo
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


