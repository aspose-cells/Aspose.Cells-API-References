---
title: "Klasse DataSorterKeyCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataSorterKeyCollection Klasse. Stellt die Schlüsselliste des DataSorters dar"
type: docs
url: /de/net/aspose.cells/datasorterkeycollection/
---
## DataSorterKeyCollection class

Stellt die Schlüsselliste des DataSorters dar.

```csharp
public class DataSorterKeyCollection : CollectionBase<DataSorterKey>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DataSorterKeyCollection](datasorterkeycollection/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/datasorterkeycollection/item/) { get; } | Liest und setzt [`DataSorterKey`](../datasorterkey/) nach Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
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

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyCollectionDemo
    {
        public static void DataSorterKeyCollectionExample()
        {
            // Instanziiere ein neues Workbook-Objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            // Hole das DataSorter‑Objekt des Arbeitsbuchs
            DataSorter sorter = workbook.DataSorter;

            // Setze die erste Reihenfolge für das DataSorter‑Objekt
            sorter.Order1 = Aspose.Cells.SortOrder.Descending;
            // Definiere den ersten Schlüssel.
            sorter.Key1 = 1; // Sorting by the second column (Score)

            // Erstelle einen Zellenbereich (Bereich)
            CellArea ca = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Sortiere Daten im angegebenen Datenbereich (A2:B4)
            sorter.Sort(worksheet.Cells, ca);

            // Greife auf die DataSorterKeyCollection zu
            DataSorterKeyCollection keys = sorter.Keys;

            // Zeige die Anzahl der Schlüssel an
            Console.WriteLine("Number of keys: " + keys.Count);

            // Greife auf den ersten Schlüssel zu und zeige seine Eigenschaften an
            DataSorterKey key = keys[0];
            Console.WriteLine("Key Index: " + key.Index);
            Console.WriteLine("Key Order: " + key.Order);

            // Speichere die Arbeitsmappe
            workbook.Save("DataSorterKeyCollectionExample.xlsx");
            workbook.Save("DataSorterKeyCollectionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [DataSorterKey](../datasorterkey/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


