---
title: "Klass HtmlTableLoadOptionCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlTableLoadOptionCollection-klass. Representerar tabellalternativen vid import av HTML"
type: docs
url: /sv/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

Representerar tabellalternativen när HTML importeras.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Hämtar [`HtmlTableLoadOption`](../htmltableloadoption/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | Anger om listobjekt ska genereras från importerade tabeller. Standardvärdet är false. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) Lägger till ett HtmlTableLoadOption i den här samlingen. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Lägg till ett HtmlTableLoadOption i listan. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Lägg till ett HtmlTableLoadOption i listan. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Lägg till ett HtmlTableLoadOption i listan. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Lägg till ett HtmlTableLoadOption i listan. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Lägg till ett HtmlTableLoadOption i listan. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Lägg till ett HtmlTableLoadOption i listan. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Lägger till ett HtmlTableLoadOption i den här samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Kom åt HtmlTableLoadOptionCollection-instansen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ställ in egenskapen TableToListObject
            tableLoadOptions.TableToListObject = true;

            // Lägg till ett nytt HtmlTableLoadOption med tabellindex
            int index1 = tableLoadOptions.Add(0);

            // Lägg till ett nytt HtmlTableLoadOption med tabell-ID
            int index2 = tableLoadOptions.Add("tableId");

            // Lägg till ett nytt HtmlTableLoadOption med tabellindex och målbladindex
            int index3 = tableLoadOptions.Add(1, 1);

            // Lägg till ett nytt HtmlTableLoadOption med tabell-ID och målbladindex
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Lägg till ett nytt HtmlTableLoadOption med tabellindex, målbladindex och ursprungsbladindex
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Lägg till ett nytt HtmlTableLoadOption med tabell-ID, målbladindex och ursprungsbladindex
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Kom åt HtmlTableLoadOption på ett specifikt index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Ställ in egenskaper för HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Läs in en HTML-fil i arbetsboken med hjälp av laddningsalternativen
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


