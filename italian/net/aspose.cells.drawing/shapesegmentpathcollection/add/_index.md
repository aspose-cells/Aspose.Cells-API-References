---
title: "ShapeSegmentPathCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeSegmentPathCollection. Aggiunge un percorso segmento nel percorso di creazione"
type: docs
url: /it/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Aggiungi un percorso di segmento nel percorso di creazione.

```csharp
public int Add(ShapePathType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ShapePathType | Il tipo di percorso. |

### Valore di ritorno

Restituisce la posizione dell'oggetto [`ShapeSegmentPath`](../../shapesegmentpath/) nell'elenco.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
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
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Visualizza il conteggio dei segmenti del percorso
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Itera attraverso ogni segmento e visualizza il suo tipo
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //aggiungi forma libera
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Salva la cartella di lavoro per osservare le modifiche della forma
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


