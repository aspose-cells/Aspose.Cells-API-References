---
title: "Classe **ListObjectCollection**"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe **Aspose.Cells.Tables.ListObjectCollection**. Rappresenta una raccolta di oggetti **ListObject** nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells.tables/listobjectcollection/
---
## ListObjectCollection class

Rappresenta una raccolta di [`ListObject`](../listobject/) oggetti nel foglio di lavoro.

```csharp
public class ListObjectCollection : CollectionBase<ListObject>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listobjectcollection/item/) { get; } | Ottiene il **ListObject** per indice. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add_1)(string, string, bool) | Aggiunge un **ListObject** al foglio di lavoro. |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add)(int, int, int, int, bool) | Aggiunge un **ListObject** al foglio di lavoro. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListObject) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListObject, IComparer&lt;ListObject&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListObject, IComparer&lt;ListObject&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListObject) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListObject[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListObject[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListObject[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListObject&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListObject&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListObject&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListObject&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject, int, int) |  |
| [RemoveAt](../../aspose.cells.tables/listobjectcollection/removeat/#removeat)(int) | Rimuovi [`ListObject`](../listobject/) per indice. (2 metodi) |
| [UpdateColumnName](../../aspose.cells.tables/listobjectcollection/updatecolumnname/)() | Aggiorna tutti i nomi delle colonne delle tabelle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectCollectionDemo
    {
        public static void ListObjectCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla ListObjectCollection del foglio di lavoro
            ListObjectCollection listObjects = worksheet.ListObjects;

            // Aggiungi un ListObject (tabella) al foglio di lavoro
            int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
            ListObject listObject = listObjects[listObjectIndex];

            // Imposta il nome del ListObject
            listObject.DisplayName = "SampleTable";

            // Popola la tabella con alcuni dati
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["D1"].PutValue("Header4");

            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row" + i + "Col1");
                worksheet.Cells[i, 1].PutValue("Row" + i + "Col2");
                worksheet.Cells[i, 2].PutValue("Row" + i + "Col3");
                worksheet.Cells[i, 3].PutValue("Row" + i + "Col4");
            }

            // Aggiorna tutti i nomi delle colonne delle tabelle
            listObjects.UpdateColumnName();

            // Salva la cartella di lavoro
            workbook.Save("ListObjectCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListObject](../listobject/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


