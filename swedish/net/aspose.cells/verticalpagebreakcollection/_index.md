---
title: "Klass VerticalPageBreakCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.VerticalPageBreakCollection-klass. Inkapslar en samling av VerticalPageBreak-objekt"
type: docs
url: /sv/net/aspose.cells/verticalpagebreakcollection/
---
## VerticalPageBreakCollection class

Inkapslar en samling av [`VerticalPageBreak`](../verticalpagebreak/) objekt.

```csharp
public class VerticalPageBreakCollection : CollectionBase<VerticalPageBreak>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/verticalpagebreakcollection/item/) { get; } | Hämtar [`VerticalPageBreak`](../verticalpagebreak/) elementet på det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add)(int) | Lägger till ett vertikalt sidbrytning i samlingen. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_3)(string) | Lägger till ett vertikalt sidbrytning i samlingen. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_1)(int, int) | Lägger till ett vertikalt sidbrytning i samlingen. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_2)(int, int, int) | Lägger till ett vertikalt sidbrytning i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VerticalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VerticalPageBreak, IComparer&lt;VerticalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VerticalPageBreak, IComparer&lt;VerticalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VerticalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VerticalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VerticalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VerticalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/verticalpagebreakcollection/removeat/#removeat)(int) | Tar bort VPageBreak-elementet med ett angivet namn. (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionDemo
    {
        public static void VerticalPageBreakCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till VerticalPageBreakCollection i kalkylbladet
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Lägg till vertikala sidbrytningar
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add("G5"); // At cell G5

            // Ta bort ett vertikalt sidbrytning på index 1
            verticalPageBreaks.RemoveAt(1);

            // Få åtkomst till och skriv ut detaljer för de vertikala sidbrytningarna
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Spara arbetsboken
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [VerticalPageBreak](../verticalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


