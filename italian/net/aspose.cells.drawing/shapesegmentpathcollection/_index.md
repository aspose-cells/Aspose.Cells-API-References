---
title: "Classe ShapeSegmentPathCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ShapeSegmentPathCollection class. Rappresenta un percorso di creazione costituito da una serie di spostamenti, linee e curve che, una volta combinati, formeranno una forma geometrica"
type: docs
url: /it/net/aspose.cells.drawing/shapesegmentpathcollection/
---
## ShapeSegmentPathCollection class

Rappresenta un percorso di creazione costituito da una serie di spostamenti, linee e curve che, combinati, formeranno una forma geometrica.

```csharp
public class ShapeSegmentPathCollection : CollectionBase<ShapeSegmentPath>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ShapeSegmentPathCollection](shapesegmentpathcollection/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapesegmentpathcollection/item/) { get; } | Ottiene l'oggetto [`ShapeSegmentPath`](../shapesegmentpath/). |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapesegmentpathcollection/add/)(ShapePathType) | Aggiungi un percorso di segmento nel percorso di creazione. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeSegmentPath) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeSegmentPath, IComparer&lt;ShapeSegmentPath&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapeSegmentPath, IComparer&lt;ShapeSegmentPath&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapeSegmentPath) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeSegmentPath[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeSegmentPath[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapeSegmentPath[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea uno ShapePath per lavorare con i segmenti
                ShapePath path = new ShapePath();

                // Inizia un nuovo percorso
                path.MoveTo(10, 10);

                // Disegna un segmento di linea
                path.LineTo(100, 100);

                // Ottieni lo ShapeSegmentPathCollection dal percorso
                ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

                // Aggiungi un segmento di percorso chiuso
                int index = segmentPaths.Add(ShapePathType.Close);

                // Visualizza le informazioni sulla raccolta
                Console.WriteLine($"Number of path segments: {segmentPaths.Count}");
                Console.WriteLine($"Added segment at index: {index}");

                // Accedi al primo segmento (proprietà di sola lettura)
                if (segmentPaths.Count > 0)
                {
                    ShapeSegmentPath firstSegment = segmentPaths[0];
                    Console.WriteLine($"First segment type: {firstSegment.Type}");
                }

                // Aggiungi la forma al foglio di lavoro
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

                // Salva la cartella di lavoro
                workbook.Save("ShapeSegmentPathCollectionDemo.xlsx");
                Console.WriteLine("ShapeSegmentPathCollection demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ShapeSegmentPathCollection demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeSegmentPath](../shapesegmentpath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


