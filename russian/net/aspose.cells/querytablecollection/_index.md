---
title: "Класс QueryTableCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.QueryTableCollection. Коллекция объектов QueryTableCollection, представляющих информацию о коллекции QueryTable."
type: docs
url: /ru/net/aspose.cells/querytablecollection/
---
## QueryTableCollection class

Коллекция объектов `QueryTableCollection`, представляющих информацию о коллекции QueryTable.

```csharp
public class QueryTableCollection : CollectionBase<QueryTable>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/querytablecollection/item/) { get; } | Получает querytable по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(QueryTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(QueryTable, IComparer&lt;QueryTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, QueryTable, IComparer&lt;QueryTable&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(QueryTable) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(QueryTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(QueryTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, QueryTable[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;QueryTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;QueryTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;QueryTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;QueryTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionDemo
    {
        public static void QueryTableCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к QueryTableCollection рабочего листа
            QueryTableCollection queryTables = worksheet.QueryTables;
            
            // Отобразить количество QueryTables в рабочем листе
            Console.WriteLine("Number of QueryTables: " + queryTables.Count);
            
            // Установить ёмкость QueryTableCollection
            queryTables.Capacity = 10;
            Console.WriteLine("Capacity of QueryTableCollection: " + queryTables.Capacity);
            
            // Предполагая, что существует хотя бы один QueryTable, получить доступ к первому QueryTable
            if (queryTables.Count > 0)
            {
                QueryTable queryTable = queryTables[0];
                Console.WriteLine("First QueryTable accessed.");
            }
            else
            {
                Console.WriteLine("No QueryTables found in the worksheet.");
            }
            
            // Сохраните книгу
            workbook.Save("QueryTableCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [QueryTable](../querytable/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


