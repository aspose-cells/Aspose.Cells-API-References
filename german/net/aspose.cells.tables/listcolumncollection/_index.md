---
title: "Klasse ListColumnCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.ListColumnCollection Klasse. Stellt eine Liste aller ListColumn‑Objekte in der Tabelle dar"
type: docs
url: /de/net/aspose.cells.tables/listcolumncollection/
---
## ListColumnCollection class

Stellt eine Liste aller [`ListColumn`](../listcolumn/) Objekte in der Tabelle dar

```csharp
public class ListColumnCollection : CollectionBase<ListColumn>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listcolumncollection/item/) { get; } | Ermittelt die ListColumn nach dem Index. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int, int) |  |
| [RemoveAt](../../aspose.cells.tables/listcolumncollection/removeat/#removeat)(int) | Entfernt [`ListColumn`](../listcolumn/) nach Index. (2 Methoden) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnCollectionDemo
    {
        public static void ListColumnCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fülle das Arbeitsblatt mit einigen Daten
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Füge ein ListObject (Tabelle) zum Arbeitsblatt hinzu
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Greift auf die ListColumnCollection des ListObject zu
            ListColumnCollection listColumns = table.ListColumns;

            // Demonstriert den Zugriff auf Eigenschaften von ListColumnCollection
            Console.WriteLine("Number of columns in the table: " + listColumns.Count);

            // Greift auf einzelne ListColumn nach Index zu
            ListColumn firstColumn = listColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);

            // Ändert die Kapazität der ListColumnCollection
            listColumns.Capacity = 10;
            Console.WriteLine("New capacity of the ListColumnCollection: " + listColumns.Capacity);

            // Speichere die Arbeitsmappe
            workbook.Save("ListColumnCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListColumn](../listcolumn/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


