---
title: "Classe ShapePathCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ShapePathCollection. Représente les informations de collection de chemins dans l'autoshape NotPrimitive"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathcollection/
---
## ShapePathCollection class

Représente les informations de collection de chemins dans l'autoshape NotPrimitive

```csharp
public class ShapePathCollection : CollectionBase<ShapePath>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells.drawing/shapepathcollection/count/) { get; } | Obtient le nombre de chemins |
| [Item](../../aspose.cells.drawing/shapepathcollection/item/) { get; } | Obtient un chemin de création. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathcollection/add/)() | Ajoute un chemin de création. |
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

### Exemples

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



            // Instanciez un nouveau classeur
            Workbook workbook = new Workbook("ShapePathCollectionExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Accédez à la ShapePathCollection de la forme d'arc
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // Ajoutez un nouveau chemin à la ShapePathCollection
                int pathIndex = shapePaths.Add();

                // Accédez au ShapePath nouvellement ajouté
                ShapePath newPath = shapePaths[pathIndex];

                // Affiche le nombre de chemins dans la ShapePathCollection
                Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
            }
            

            // Enregistrez le classeur
            workbook.Save("ShapePathCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePath](../shapepath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


