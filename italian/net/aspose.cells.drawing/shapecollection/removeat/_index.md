---
title: "ShapeCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Rimuove la forma"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Rimuovi la forma.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice della forma. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi la prima forma rettangolare
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Aggiungi la seconda forma rettangolare
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Rimuove la prima forma all'indice 0
            shapes.RemoveAt(0);

            // Salva la cartella di lavoro
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


