---
title: "Класс ContentTypePropertyCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Properties.ContentTypePropertyCollection. Коллекция объектов ContentTypeProperty, представляющих дополнительную информацию."
type: docs
url: /ru/net/aspose.cells.properties/contenttypepropertycollection/
---
## ContentTypePropertyCollection class

Коллекция объектов [`ContentTypeProperty`](../contenttypeproperty/), представляющих дополнительную информацию.

```csharp
public class ContentTypePropertyCollection : CollectionBase<ContentTypeProperty>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/contenttypepropertycollection/item/) { get; } | Получает свойство типа содержимого по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add)(string, string) | Добавляет информацию о свойстве типа содержимого. |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add_1)(string, string, string) | Добавляет информацию о свойстве типа содержимого. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ContentTypeProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ContentTypeProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ContentTypeProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ContentTypeProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ContentTypeProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyCollectionDemo
    {
        public static void ContentTypePropertyCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Добавить новое свойство в ContentTypePropertyCollection
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Доступ к ContentTypePropertyCollection
            ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;

            // Отображение количества свойств
            Console.WriteLine("Number of ContentTypeProperties: " + contentTypeProperties.Count);

            // Доступ к конкретному свойству по индексу
            ContentTypeProperty property = contentTypeProperties[0];
            Console.WriteLine("Property Name: " + property.Name);
            Console.WriteLine("Property Value: " + property.Value);
            Console.WriteLine("Property Type: " + property.Type);

            // Изменение ёмкости коллекции
            contentTypeProperties.Capacity = 10;
            Console.WriteLine("New Capacity: " + contentTypeProperties.Capacity);

            // Сохраните файл Excel
            workbook.Save("ContentTypePropertyCollectionExample.xlsx");
            workbook.Save("ContentTypePropertyCollectionExample.pdf");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ContentTypeProperty](../contenttypeproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


