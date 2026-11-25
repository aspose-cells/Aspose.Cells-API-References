---
title: "ShapePathCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathCollection. Ottiene un percorso di creazione"
type: docs
url: /it/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Restituisce un percorso di creazione.

```csharp
public ShapePath this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

Restituisce l'oggetto [`ShapePath`](../../shapepath/).

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma personalizzata (forma non primitiva) con i parametri corretti
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // Accedi alla ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Aggiungi un nuovo percorso
            int pathIndex = shapePaths.Add();

            // Accedi al percorso usando la proprietà Item
            ShapePath newPath = shapePaths[pathIndex];

            // Informazioni di output
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Salva la cartella di lavoro
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


