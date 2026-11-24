---
title: "Klasse ListObjectCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.ListObjectCollection Klasse. Stellt eine Sammlung von ListObject-Objekten im Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells.tables/listobjectcollection/
---
## ListObjectCollection class

Stellt eine Sammlung von [`ListObject`](../listobject/) Objekten im Arbeitsblatt dar.

```csharp
public class ListObjectCollection : CollectionBase<ListObject>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listobjectcollection/item/) { get; } | Ruft das ListObject nach Index ab. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add_1)(string, string, bool) | Fügt ein ListObject dem Arbeitsblatt hinzu. |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add)(int, int, int, int, bool) | Fügt ein ListObject dem Arbeitsblatt hinzu. |
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
| [RemoveAt](../../aspose.cells.tables/listobjectcollection/removeat/#removeat)(int) | Entfernt [`ListObject`](../listobject/) nach Index. (2 Methoden) |
| [UpdateColumnName](../../aspose.cells.tables/listobjectcollection/updatecolumnname/)() | Aktualisiert alle Spaltennamen der Tabellen. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf die ListObjectCollection des Arbeitsblatts zu
            ListObjectCollection listObjects = worksheet.ListObjects;

            // Füge ein ListObject (Tabelle) zum Arbeitsblatt hinzu
            int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
            ListObject listObject = listObjects[listObjectIndex];

            // Setzen Sie den Namen des ListObject
            listObject.DisplayName = "SampleTable";

            // Füllen Sie die Tabelle mit einigen Daten
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

            // Aktualisieren Sie alle Spaltennamen der Tabellen
            listObjects.UpdateColumnName();

            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectCollectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListObject](../listobject/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


