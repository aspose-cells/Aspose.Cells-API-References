---
title: "Klass RangeCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.RangeCollection-klass. Inkapslar en samling av Range-objekt"
type: docs
url: /sv/net/aspose.cells/rangecollection/
---
## RangeCollection class

Inkapslar en samling av [`Range`](../range/) objekt.

```csharp
public class RangeCollection : CollectionBase<Range>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/rangecollection/item/) { get; } | Hämtar [`Range`](../range/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/rangecollection/add/)(Range) | (**Föråldrad.**) Lägger till ett [`Range`](../range/)‑objekt i samlingen. |
| [AddRange](../../aspose.cells/rangecollection/addrange/)(Range) | Lägger till ett [`Range`](../range/)‑objekt i samlingen. |
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

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa områden och lägg till dem i kalkylbladet
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            
            // Hämta RangeCollection från kalkylbladet
            RangeCollection rangeCollection = worksheet.Cells.Ranges;
            
            // Lägg till områden i samlingen
            rangeCollection.Add(range1);
            rangeCollection.Add(range2);

            // Skapa en annan RangeCollection för jämförelse
            RangeCollection compareCollection = worksheet.Cells.Ranges;
            compareCollection.Add(worksheet.Cells.CreateRange("A1:B2"));
            compareCollection.Add(worksheet.Cells.CreateRange("C3:D4"));

            // Jämför de två RangeCollections
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

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Range](../range/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


