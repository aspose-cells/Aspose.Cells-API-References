---
title: "ShapeCollection.Group"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Raggruppa le forme"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Raggruppa le forme.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| groupItems | Shape[] | gli elementi del gruppo. |

### Valore di ritorno

Restituisce la forma del gruppo.

### Osservazioni

La forma in groupItems non dovrebbe essere raggruppata. La forma deve trovarsi in questa collezione Shapes.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi la prima forma rettangolare
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Aggiungi la seconda forma rettangolare
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Crea un array con le forme da raggruppare
            Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };

            // Raggruppa le forme
            GroupShape groupShape = shapes.Group(shapesArr);

            // Salva la cartella di lavoro
            workbook.Save("GroupShapesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


