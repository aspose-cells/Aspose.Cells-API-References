---
title: "Класс ExternalConnectionCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExternalConnections.ExternalConnectionCollection. Определяет коллекцию ExternalConnection"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

Определяет коллекцию [`ExternalConnection`](../externalconnection/)

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item/) { get; } | Получает элемент [`ExternalConnection`](../externalconnection/) по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ExternalConnection) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ExternalConnection, IComparer&lt;ExternalConnection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ExternalConnection, IComparer&lt;ExternalConnection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ExternalConnection) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ExternalConnection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ExternalConnection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ExternalConnection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ExternalConnection&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ExternalConnection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/)(int) | Получает элемент [`ExternalConnection`](../externalconnection/) с указанным id. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionDemo
    {
        public static void ExternalConnectionCollectionExample()
        {
            // Загрузите существующую книгу, содержащую внешние соединения
            Workbook workbook = new Workbook("ExternalConnectionCollectionExample_original.xlsx");

            // Получите коллекцию внешних соединений из книги
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Итерируйтесь по внешним соединениям и выводите их идентификаторы
            for (int i = 0; i < dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Получить идентификатор внешнего соединения
                Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
            }

            // Пример доступа к конкретному внешнему соединению по ID
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($"Found External Connection with ID {specificConnId}");
                // Здесь вы можете получить доступ и изменить свойства конкретного соединения
                specificConn.Name = "Updated Connection Name";
            }

            // Сохраните книгу, если были внесены изменения
            workbook.Save("ExternalConnectionCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


