---
title: "Klasse RangeCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.RangeCollection Klasse. Kapselt eine Sammlung von Range‑Objekten"
type: docs
url: /de/net/aspose.cells/rangecollection/
---
## RangeCollection class

Kapselt eine Sammlung von [`Range`](../range/) Objekten.

```csharp
public class RangeCollection : CollectionBase<Range>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/rangecollection/item/) { get; } | Liest das [`Range`](../range/) Element am angegebenen Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/rangecollection/add/)(Range) | (**Obsolete.**) Fügt ein [`Range`](../range/) Element zur Sammlung hinzu. |
| [AddRange](../../aspose.cells/rangecollection/addrange/)(Range) | Fügt ein [`Range`](../range/) Element zur Sammlung hinzu. |
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

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereiche erstellen und zum Arbeitsblatt hinzufügen
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            
            // Die RangeCollection vom Arbeitsblatt abrufen
            RangeCollection rangeCollection = worksheet.Cells.Ranges;
            
            // Bereiche zur Sammlung hinzufügen
            rangeCollection.Add(range1);
            rangeCollection.Add(range2);

            // Eine weitere RangeCollection zum Vergleich erstellen
            RangeCollection compareCollection = worksheet.Cells.Ranges;
            compareCollection.Add(worksheet.Cells.CreateRange("A1:B2"));
            compareCollection.Add(worksheet.Cells.CreateRange("C3:D4"));

            // Die beiden RangeCollections vergleichen
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

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Range](../range/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


