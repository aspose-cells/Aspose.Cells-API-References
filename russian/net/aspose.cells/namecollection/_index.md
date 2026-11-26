---
title: "Класс NameCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.NameCollection. Представляет коллекцию всех объектов Name в таблице."
type: docs
url: /ru/net/aspose.cells/namecollection/
---
## NameCollection class

Представляет коллекцию всех объектов [`Name`](../name/) в таблице.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Получает элемент [`Name`](../name/) по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Определяет новое имя. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Удаляет все определённые имена, которые не используются в формулах и источнике данных. Если определённое имя используется, мы только устанавливаем Name.ReferTo в null и скрываем его. (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Получает все определённые имена по области. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Удалить имя. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Удалить массив имён |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Удалить имя по конкретному индексу. (2 метода) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Удалить дублирующиеся определённые имена |
| [Sort](../../aspose.cells/namecollection/sort/)() | Сортирует определённые имена. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к коллекции листов
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Получить доступ к коллекции имён
            NameCollection names = worksheets.Names;
            
            // Добавить новое имя в коллекцию
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Установить свойство refers to для имени
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Получить доступ и изменить свойства имени
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Добавить ещё одно имя
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Удалить имя по тексту
            names.Remove("AnotherNamedRange");
            
            // Удалить имя по индексу
            names.RemoveAt(nameIndex);
            
            // Очистить все имена
            names.Clear();
            
            // Сохраните книгу
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


