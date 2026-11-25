---
title: "ShapeCollection.DeleteShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Elimina una forma. Se la forma è nel gruppo o è una forma commento non verrà eliminata"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Elimina una forma. Se la forma è nel gruppo o è una forma di commento, non verrà eliminata.

```csharp
public void DeleteShape(Shape shape)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| shape | Forma |  |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi la prima forma rettangolare
            Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Aggiungi la seconda forma rettangolare
            Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Elimina la prima forma
            shapes.DeleteShape(firstShape);

            // Salva la cartella di lavoro
            workbook.Save("DeleteShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


