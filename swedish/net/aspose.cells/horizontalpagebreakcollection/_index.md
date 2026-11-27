---
title: "Klass HorizontalPageBreakCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HorizontalPageBreakCollection-klassen. Inkapslar en samling av HorizontalPageBreak-objekt"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreakcollection/
---
## HorizontalPageBreakCollection class

Inkapslar en samling av [`HorizontalPageBreak`](../horizontalpagebreak/) objekt.

```csharp
public class HorizontalPageBreakCollection : CollectionBase<HorizontalPageBreak>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/horizontalpagebreakcollection/item/) { get; } | Hämtar [`HorizontalPageBreak`](../horizontalpagebreak/) elementet vid det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add)(int) | Lägger till ett horisontellt sidbrytning i samlingen. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_3)(string) | Lägger till ett horisontellt sidbrytning i samlingen. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_1)(int, int) | Lägger till ett horisontellt sidbrytning i samlingen. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_2)(int, int, int) | Lägger till ett horisontellt sidbrytning i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HorizontalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HorizontalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/horizontalpagebreakcollection/removeat/#removeat)(int) | Tar bort HPageBreak-elementet med ett angivet namn. (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakCollectionDemo
    {
        public static void HorizontalPageBreakCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett horisontellt sidbryt vid rad 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Lägg till ett horisontellt sidbryt vid rad 10, med start från kolumn 1 till kolumn 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Lägg till ett horisontellt sidbryt vid rad 15, med start från kolumn 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Lägg till ett horisontellt sidbryt vid cell "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Ta bort den första horisontella sidbrytningen
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Spara arbetsboken
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HorizontalPageBreak](../horizontalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


