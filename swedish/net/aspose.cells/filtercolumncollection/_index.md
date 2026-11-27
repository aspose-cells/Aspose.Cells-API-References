---
title: "Class FilterColumnCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FilterColumnCollection class. En samling av Filter-objekt som representerar alla filter i ett autofilterområde"
type: docs
url: /sv/net/aspose.cells/filtercolumncollection/
---
## FilterColumnCollection class

En samling av Filter‑objekt som representerar alla filter i ett autofilterområde.

```csharp
public class FilterColumnCollection : CollectionBase<FilterColumn>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/filtercolumncollection/item/) { get; } | Hämtar [`FilterColumn`](../filtercolumn/) objektet vid det speciella fältet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FilterColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FilterColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FilterColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [GetByIndex](../../aspose.cells/filtercolumncollection/getbyindex/)(int) | Returnerar ett enda Filter-objekt från en samling. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int, int) |  |
| [RemoveAt](../../aspose.cells/filtercolumncollection/removeat/#removeat)(int) | (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnCollectionDemo
    {
        public static void FilterColumnCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att filtrera
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(22);

            // Skapa ett AutoFilter
            worksheet.AutoFilter.Range = "A1:B4";

            // Hämta FilterColumnCollection
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            // Lägg till ett filter i den andra kolumnen (Age)
            worksheet.AutoFilter.AddFilter(1, "25");

            // Tillämpa filtret
            worksheet.AutoFilter.Refresh();

            // Kom åt och manipulera FilterColumnCollection
            Console.WriteLine("Number of filters applied: " + filterColumns.Count);

            // Hämta den första filterkolumnen
            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine("Filter applied on column index: " + filterColumn.FieldIndex);

            // Ta bort filtret
            filterColumns.RemoveAt(0);
            worksheet.AutoFilter.Refresh();

            // Spara arbetsboken
            workbook.Save("FilterColumnCollectionExample.xlsx");
            workbook.Save("FilterColumnCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FilterColumn](../filtercolumn/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


