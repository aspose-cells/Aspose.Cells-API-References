---
title: "Класс WebExtensionBindingCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.WebExtensions.WebExtensionBindingCollection class. Представляет список отношений привязки между надстройкой Office и данными в документе"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionbindingcollection/
---
## WebExtensionBindingCollection class

Представляет список связей привязки между надстройкой Office и данными в документе.

```csharp
public class WebExtensionBindingCollection : CollectionBase<WebExtensionBinding>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WebExtensionBindingCollection](webextensionbindingcollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionbindingcollection/item/) { get; } | Получает связь привязки веб-расширения по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionbindingcollection/add/)() | Добавляет связь привязки между надстройкой Office и данными в документе. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionBinding) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionBinding[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать экземпляр WebExtensionBindingCollection
                WebExtensionBindingCollection bindings = new WebExtensionBindingCollection();
                
                // Добавить новую привязку
                int index = bindings.Add();
                
                // Получить доступ к привязке через индексатор
                WebExtensionBinding binding = bindings[index];
                
                // Установить свойства привязки (при условии, что эти свойства существуют на основе примеров справки)
                binding.Id = "binding1";
                binding.Type = "table";
                binding.Appref = "Sheet1!A1:B5";
                
                // Отобразить базовую информацию
                Console.WriteLine($"Created binding with ID: {binding.Id}");
                Console.WriteLine($"Total bindings in collection: {bindings.Count}");
                
                // Сохраните книгу
                workbook.Save("WebExtensionBindingCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBindingCollection: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionBinding](../webextensionbinding/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


