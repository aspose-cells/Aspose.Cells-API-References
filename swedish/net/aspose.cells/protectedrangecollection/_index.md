---
title: "Klass ProtectedRangeCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ProtectedRangeCollection-klass. Inkapslar en samling av ProtectedRange-objekt"
type: docs
url: /sv/net/aspose.cells/protectedrangecollection/
---
## ProtectedRangeCollection class

Inkapslar en samling av [`ProtectedRange`](../protectedrange/) objekt.

```csharp
public class ProtectedRangeCollection : CollectionBase<ProtectedRange>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/protectedrangecollection/item/) { get; } | Hämtar [`ProtectedRange`](../protectedrange/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/protectedrangecollection/add/)(string, int, int, int, int) | Lägger till ett [`ProtectedRange`](../protectedrange/) objekt i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ProtectedRange) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ProtectedRange, IComparer&lt;ProtectedRange&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ProtectedRange, IComparer&lt;ProtectedRange&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ProtectedRange) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ProtectedRange[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ProtectedRange[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ProtectedRange[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ProtectedRange&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ProtectedRange&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ProtectedRange&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ProtectedRange&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ProtectedRange&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ProtectedRange&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ProtectedRange) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ProtectedRange, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ProtectedRange, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ProtectedRange) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ProtectedRange, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ProtectedRange, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av skyddade områden
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;

            // Lägg till ett nytt skyddat område
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = protectedRanges[index];
            protectedRange.Password = "1234";

            // Lägg till ett annat skyddat område
            index = protectedRanges.Add("AnotherRange", 3, 3, 5, 5);
            protectedRange = protectedRanges[index];
            protectedRange.Password = "5678";

            // Visa information om skyddade områden
            Console.WriteLine("Protected Ranges in Worksheet:");
            foreach (ProtectedRange range in protectedRanges)
            {
                Console.WriteLine($"Name: {range.Name}");
                Console.WriteLine($"Area: {range.CellArea.StartRow},{range.CellArea.StartColumn} to {range.CellArea.EndRow},{range.CellArea.EndColumn}");
                Console.WriteLine($"Password Protected: {!string.IsNullOrEmpty(range.Password)}");
                Console.WriteLine();
            }

            // Spara arbetsboken
            workbook.Save("ProtectedRangesDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ProtectedRange](../protectedrange/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


