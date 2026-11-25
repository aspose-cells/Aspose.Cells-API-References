---
title: "Classe DataSorterKeyCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataSorterKeyCollection. Rappresenta l'elenco delle chiavi del data sorter"
type: docs
url: /it/net/aspose.cells/datasorterkeycollection/
---
## DataSorterKeyCollection class

Rappresenta l'elenco delle chiavi del DataSorter.

```csharp
public class DataSorterKeyCollection : CollectionBase<DataSorterKey>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DataSorterKeyCollection](datasorterkeycollection/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/datasorterkeycollection/item/) { get; } | Ottiene e imposta [`DataSorterKey`](../datasorterkey/) per indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
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

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyCollectionDemo
    {
        public static void DataSorterKeyCollectionExample()
        {
            // Istanzia un nuovo oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            // Ottieni l'oggetto DataSorter della cartella di lavoro
            DataSorter sorter = workbook.DataSorter;

            // Imposta il primo ordine per l'oggetto DataSorter
            sorter.Order1 = Aspose.Cells.SortOrder.Descending;
            // Definisci la prima chiave
            sorter.Key1 = 1; // Sorting by the second column (Score)

            // Crea un'area di celle (intervallo)
            CellArea ca = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Ordina i dati nell'intervallo specificato (A2:B4)
            sorter.Sort(worksheet.Cells, ca);

            // Accedi a DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Visualizza il conteggio delle chiavi
            Console.WriteLine("Number of keys: " + keys.Count);

            // Accedi alla prima chiave e visualizza le sue proprietà
            DataSorterKey key = keys[0];
            Console.WriteLine("Key Index: " + key.Index);
            Console.WriteLine("Key Order: " + key.Order);

            // Salva la cartella di lavoro
            workbook.Save("DataSorterKeyCollectionExample.xlsx");
            workbook.Save("DataSorterKeyCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [DataSorterKey](../datasorterkey/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


