---
title: "ShapeSegmentPathCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeSegmentPathCollection. Ottiene l'oggetto ShapeSegmentPath"
type: docs
url: /it/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Ottiene l'oggetto [`ShapeSegmentPath`](../../shapesegmentpath/).

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

Restituisce un oggetto [`ShapeSegmentPath`](../../shapesegmentpath/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Inizia un nuovo percorso
            path.MoveTo(10, 10);

            // Disegna un segmento di linea
            path.LineTo(100, 100);

            // Accedi alla proprietà PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Visualizza il conteggio dei segmenti del percorso
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Dimostra la lettura della proprietà Item
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //aggiungi forma libera
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Salva la cartella di lavoro
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


