---
title: "Klass DataSorterKeyCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataSorterKeyCollection-klass. Representerar nyckellistan för datasortering"
type: docs
url: /sv/net/aspose.cells/datasorterkeycollection/
---
## DataSorterKeyCollection class

Representerar nyckellistan för datasorteringen.

```csharp
public class DataSorterKeyCollection : CollectionBase<DataSorterKey>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DataSorterKeyCollection](datasorterkeycollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/datasorterkeycollection/item/) { get; } | Hämtar och sätter [`DataSorterKey`](../datasorterkey/) efter index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataSorterKey) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataSorterKey, IComparer&lt;DataSorterKey&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DataSorterKey, IComparer&lt;DataSorterKey&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DataSorterKey) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataSorterKey[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataSorterKey[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DataSorterKey[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DataSorterKey&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DataSorterKey&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyCollectionDemo
    {
        public static void DataSorterKeyCollectionExample()
        {
            // Instansiera ett nytt Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            // Hämta arbetsbokens DataSorter‑objekt
            DataSorter sorter = workbook.DataSorter;

            // Ange den första ordningen för DataSorter‑objektet
            sorter.Order1 = Aspose.Cells.SortOrder.Descending;
            // Definiera den första nyckeln
            sorter.Key1 = 1; // Sorting by the second column (Score)

            // Skapa ett cellområde (intervall)
            CellArea ca = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Sortera data i det angivna dataintervallet (A2:B4)
            sorter.Sort(worksheet.Cells, ca);

            // Få åtkomst till DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Visa antalet nycklar
            Console.WriteLine("Number of keys: " + keys.Count);

            // Få åtkomst till den första nyckeln och visa dess egenskaper
            DataSorterKey key = keys[0];
            Console.WriteLine("Key Index: " + key.Index);
            Console.WriteLine("Key Order: " + key.Order);

            // Spara arbetsboken
            workbook.Save("DataSorterKeyCollectionExample.xlsx");
            workbook.Save("DataSorterKeyCollectionExample.pdf");
            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [DataSorterKey](../datasorterkey/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


