---
title: "Класс CustomDocumentPropertyCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Properties.CustomDocumentPropertyCollection. Коллекция пользовательских свойств документа"
type: docs
url: /ru/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

Коллекция пользовательских свойств документа.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Возвращает объект [`DocumentProperty`](../documentproperty/) по индексу.(Наследовано от [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Возвращает объект [`DocumentProperty`](../documentproperty/) по имени свойства.(Наследовано от [`DocumentPropertyCollection`](../documentpropertycollection/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add)(string, bool) | Создаёт новое пользовательское свойство документа типа данных **PropertyType.Boolean**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_3)(string, DateTime) | Создаёт новое пользовательское свойство документа типа данных **PropertyType.DateTime**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_1)(string, double) | Создаёт новое пользовательское свойство документа типа данных **PropertyType.Float**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_2)(string, int) | Создаёт новое пользовательское свойство документа типа данных **PropertyType.Number**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_4)(string, string) | Создаёт новое пользовательское свойство документа типа данных **PropertyType.String**. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/)(string, string) | Создаёт новое пользовательское свойство документа, которое связывается с содержимым. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/)(string) | Возвращает true, если свойство с указанным именем существует в коллекции.(Наследовано от [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DocumentProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DocumentProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty) |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/)(string) | Получает индекс свойства по имени.(Наследовано от [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Удаляет свойство с указанным именем из коллекции.(Наследовано от [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/)(int) | Удаляет свойство по указанному индексу. (2 метода) |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/)() | Обновляет значения всех пользовательских свойств, связанных с содержимым (использует значение ячейки связанного диапазона для обновления значения пользовательского свойства). |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/)() | Обновляет все диапазоны, связанные с пользовательскими свойствами (использует значение пользовательского свойства документа для обновления значения ячейки связанного диапазона). |

### Примечания

Каждый объект [`DocumentProperty`](../documentproperty/) представляет пользовательское свойство контейнерного документа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomDocumentPropertyCollectionDemo
    {
        public static void CustomDocumentPropertyCollectionExample()
        {
            // Создайте объект Workbook
            Workbook workbook = new Workbook();

            // Получите список всех пользовательских свойств документа Excel
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Добавить пользовательские свойства документа
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Добавить связанное пользовательское свойство документа
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Обновить значения связанных свойств
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Доступ к пользовательским свойствам документа
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Вывести пользовательские свойства документа
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Сохраните книгу
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
    }
}
```

### См. также

* class [DocumentPropertyCollection](../documentpropertycollection/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


