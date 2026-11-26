---
title: "Класс ListObjectCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.ListObjectCollection. Представляет коллекцию объектов ListObject в листе"
type: docs
url: /ru/net/aspose.cells.tables/listobjectcollection/
---
## ListObjectCollection class

Представляет коллекцию объектов [`ListObject`](../listobject/) в листе.

```csharp
public class ListObjectCollection : CollectionBase<ListObject>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listobjectcollection/item/) { get; } | Получает объект ListObject по индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add_1)(string, string, bool) | Добавляет объект ListObject в лист. |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add)(int, int, int, int, bool) | Добавляет объект ListObject в лист. |
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
| [RemoveAt](../../aspose.cells.tables/listobjectcollection/removeat/#removeat)(int) | Удалить [`ListObject`](../listobject/) по индексу. (2 метода) |
| [UpdateColumnName](../../aspose.cells.tables/listobjectcollection/updatecolumnname/)() | Обновить все названия столбцов таблиц. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ListObjectCollection рабочего листа.
            ListObjectCollection listObjects = worksheet.ListObjects;

            // Добавить объект ListObject (таблицу) в лист
            int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
            ListObject listObject = listObjects[listObjectIndex];

            // Установить имя ListObject.
            listObject.DisplayName = "SampleTable";

            // Заполнить таблицу некоторыми данными.
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

            // Обновить все имена столбцов таблиц.
            listObjects.UpdateColumnName();

            // Сохраните книгу
            workbook.Save("ListObjectCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListObject](../listobject/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


