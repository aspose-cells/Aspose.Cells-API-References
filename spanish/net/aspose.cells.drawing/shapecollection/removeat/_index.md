---
title: "ShapeCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Elimina la forma"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Elimina la forma.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de la forma. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
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

            // Eliminar la primera forma en el índice 0
            shapes.RemoveAt(0);

            // Guarda el libro de trabajo
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


