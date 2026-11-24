---
title: "Klasse ShapePathCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePathCollection Klasse. Stellt Pfadsammlungsinformationen in NotPrimitive Autoform dar"
type: docs
url: /de/net/aspose.cells.drawing/shapepathcollection/
---
## ShapePathCollection class

Stellt Pfadsammlungsinformationen in NotPrimitive-Autoshape dar

```csharp
public class ShapePathCollection : CollectionBase<ShapePath>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells.drawing/shapepathcollection/count/) { get; } | Liefert die Anzahl der Pfade |
| [Item](../../aspose.cells.drawing/shapepathcollection/item/) { get; } | Liefert einen Erstellungs-Pfad. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathcollection/add/)() | Füge einen Erstellungs-Pfad hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapePath) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapePath, IComparer&lt;ShapePath&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapePath, IComparer&lt;ShapePath&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapePath) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapePath[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapePath[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapePath[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapePath&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapePath&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapePath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapePath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapePath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapePath&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapePath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapePath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapePath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapePath&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePath) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePath, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePath, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePath) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePath, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePath, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathCollectionDemo
    {
        public static void ShapePathCollectionExample()
        {



            // Instanziieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook("ShapePathCollectionExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Greife auf die ShapePathCollection der Bogenform zu
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // Füge einen neuen Pfad zur ShapePathCollection hinzu
                int pathIndex = shapePaths.Add();

                // Greife auf den neu hinzugefügten ShapePath zu
                ShapePath newPath = shapePaths[pathIndex];

                // Zeige die Anzahl der Pfade in der ShapePathCollection an
                Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
            }
            

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePathCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePath](../shapepath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


