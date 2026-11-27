---
title: "Klassen NameCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.NameCollection‑klass. Representerar en samling av alla Name‑objekt i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/namecollection/
---
## NameCollection class

Representerar en samling av alla [`Name`](../name/) objekt i kalkylbladet.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Hämtar [`Name`](../name/) elementet på det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Definierar ett nytt namn. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Ta bort alla definierade namn som inte refereras av formlerna och datakällan. Om det definierade namnet refereras, sätter vi bara Name.ReferTo till null och döljer dem. (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Hämtar alla definierade namn efter omfång. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Ta bort namnet. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Ta bort en array av namn |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Ta bort namnet på det specifika indexet. (2 metoder) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Ta bort de duplicerade definierade namnen |
| [Sort](../../aspose.cells/namecollection/sort/)() | Sorterar definierade namn. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsbladsamlingen
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Åtkomst till namnsamlingen
            NameCollection names = worksheets.Names;
            
            // Lägg till ett nytt namn i samlingen
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Ställ in referens-egenskapen för namnet
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Åtkomst till och ändra egenskaperna för namnet
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Lägg till ett annat namn
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Ta bort ett namn efter text
            names.Remove("AnotherNamedRange");
            
            // Ta bort ett namn efter index
            names.RemoveAt(nameIndex);
            
            // Rensa alla namn
            names.Clear();
            
            // Spara arbetsboken
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


