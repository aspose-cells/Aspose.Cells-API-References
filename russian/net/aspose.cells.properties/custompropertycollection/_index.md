---
title: "Класс CustomPropertyCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Properties.CustomPropertyCollection. Коллекция объектов CustomProperty, представляющих дополнительную информацию"
type: docs
url: /ru/net/aspose.cells.properties/custompropertycollection/
---
## CustomPropertyCollection class

Коллекция объектов [`CustomProperty`](../customproperty/), представляющих дополнительную информацию.

```csharp
public class CustomPropertyCollection : CollectionBase<CustomProperty>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/custompropertycollection/item/) { get; } | Получает пользовательское свойство по конкретному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.properties/custompropertycollection/add/)(string, string) | Добавляет информацию о пользовательском свойстве. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomProperty, IComparer&lt;CustomProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomProperty, IComparer&lt;CustomProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyCollectionDemo
    {
        public static void CustomPropertyCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к CustomPropertyCollection листа
            CustomPropertyCollection customProperties = worksheet.CustomProperties;

            // Добавить пользовательские свойства
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            // Получить доступ и вывести пользовательские свойства
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Сохраните книгу
            workbook.Save("CustomPropertyCollectionExample.xlsx");
            workbook.Save("CustomPropertyCollectionExample.pdf");
            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomProperty](../customproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


