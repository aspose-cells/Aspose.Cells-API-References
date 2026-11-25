---
title: "ShapeCollection.Ungroup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Separa gli elementi della forma"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Separa gli elementi della forma.

```csharp
public void Ungroup(GroupShape group)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| gruppo | GroupShape | La forma di gruppo. |

### Osservazioni

Se la forma di gruppo è raggruppata da un'altra forma di gruppo, non verrà eseguita alcuna operazione.

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi la prima forma rettangolare
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Aggiungi la seconda forma rettangolare
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Crea un array di forme da raggruppare
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Raggruppa le forme
            GroupShape groupShape = shapes.Group(shapesArr);

            // Separa la forma di gruppo
            shapes.Ungroup(groupShape);
        }
    }
}
```

### Vedi anche

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


