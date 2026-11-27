---
title: "Klass CellWatchCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellWatchCollection-klass. Representerar samlingen av celler i detta kalkylblad som övervakas i övervakningsfönstret"
type: docs
url: /sv/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

Representerar samlingen av celler i detta kalkylblad som övervakas i 'watch window'.

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CellWatchCollection](cellwatchcollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item/) { get; } | Hämtar och anger [`CellWatch`](../cellwatch/) efter index. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add/#add_1)(string) | Lägger till [`CellWatch`](../cellwatch/) med cellens namn. |
| [Add](../../aspose.cells/cellwatchcollection/add/#add)(int, int) | Lägger till [`CellWatch`](../cellwatch/) med en rad och en kolumn. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionDemo
    {
        public static void CellWatchCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Hämta det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till Cell Watch‑objekt i övervakningsfönstret
            int watchIndex = sheet.CellWatches.Add("B2");
            
            // Åtkomst till CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Åtkomst till det tillagda CellWatch-objektet
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // Visa egenskaperna för CellWatch-objektet
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Ändra egenskaperna för CellWatch-objektet
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A2";
            
            // Visa de ändrade egenskaperna för CellWatch-objektet
            Console.WriteLine("Modified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Spara arbetsboken
            workbook.Save("CellWatchCollectionExample.xlsx");
            workbook.Save("CellWatchCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CellWatch](../cellwatch/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


