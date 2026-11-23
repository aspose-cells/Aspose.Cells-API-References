---
title: "Classe RangeCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.RangeCollection. Encapsule une collection d'objets Range"
type: docs
url: /fr/net/aspose.cells/rangecollection/
---
## RangeCollection class

Encapsule une collection d'objets [`Range`](../range/).

```csharp
public class RangeCollection : CollectionBase<Range>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/rangecollection/item/) { get; } | Obtient l'élément [`Range`](../range/) à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/rangecollection/add/)(Range) | (**Obsolète.**) Ajoute un élément [`Range`](../range/) à la collection. |
| [AddRange](../../aspose.cells/rangecollection/addrange/)(Range) | Ajoute un élément [`Range`](../range/) à la collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Range) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Range, IComparer&lt;Range&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Range, IComparer&lt;Range&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Range) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Range[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Range[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Range[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Range&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Range&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Range&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Range&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Range&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Range&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Range, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Range, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des plages et les ajouter à la feuille de calcul
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            
            // Obtenez la RangeCollection à partir de la feuille de calcul
            RangeCollection rangeCollection = worksheet.Cells.Ranges;
            
            // Ajoutez des plages à la collection
            rangeCollection.Add(range1);
            rangeCollection.Add(range2);

            // Créez une autre RangeCollection pour la comparaison
            RangeCollection compareCollection = worksheet.Cells.Ranges;
            compareCollection.Add(worksheet.Cells.CreateRange("A1:B2"));
            compareCollection.Add(worksheet.Cells.CreateRange("C3:D4"));

            // Comparez les deux RangeCollections
            bool areEqual = CompareRangeCollections(rangeCollection, compareCollection);
            Console.WriteLine("RangeCollections are equal: " + areEqual);
        }

        private static bool CompareRangeCollections(RangeCollection src, RangeCollection dest)
        {
            if (src.Count != dest.Count)
                return false;

            for (int i = 0; i < src.Count; i++)
            {
                bool foundMatch = false;
                Aspose.Cells.Range srcRange = src[i];
                
                foreach (Aspose.Cells.Range destRange in dest)
                {
                    if (srcRange.FirstRow == destRange.FirstRow &&
                        srcRange.FirstColumn == destRange.FirstColumn &&
                        srcRange.RowCount == destRange.RowCount &&
                        srcRange.ColumnCount == destRange.ColumnCount)
                    {
                        foundMatch = true;
                        break;
                    }
                }
                
                if (!foundMatch)
                    return false;
            }
            
            return true;
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Range](../range/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


