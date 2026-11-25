---
title: "ShapeCollection.Remove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Rimuove la forma"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Rimuovi la forma.

```csharp
public void Remove(Shape shape)
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
    public class ShapeCollectionMethodRemoveWithShapeDemo
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

            // Ottieni la prima forma per nome o indice
            Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
            
            if (shapeToRemove != null)
            {
                // Rimuovi la forma dalla collezione
                shapes.Remove(shapeToRemove);
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeRemoveDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


