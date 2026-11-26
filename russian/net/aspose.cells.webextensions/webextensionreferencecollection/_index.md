---
title: "Класс WebExtensionReferenceCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WebExtensions.WebExtensionReferenceCollection. Представляет список ссылок веб‑расширения"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionreferencecollection/
---
## WebExtensionReferenceCollection class

Представляет список ссылок на веб‑расширения.

```csharp
public class WebExtensionReferenceCollection : CollectionBase<WebExtensionReference>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WebExtensionReferenceCollection](webextensionreferencecollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionreferencecollection/item/) { get; } | Получает веб‑расширение по конкретному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionreferencecollection/add/)() | Добавляет пустую ссылку на веб‑расширение. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionReference, IComparer&lt;WebExtensionReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionReference, IComparer&lt;WebExtensionReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionReference) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionReference[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionReference[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionReference[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionReference&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionReference) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionReference, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionReference, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionReference) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionReference, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionReference, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceCollectionDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр WebExtensionReferenceCollection
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Добавьте новую ссылку на веб‑расширение
                int index = references.Add();
                
                // Получите доступ к добавленной ссылке (только для чтения)
                WebExtensionReference reference = references[index];
                
                Console.WriteLine($"Added web extension reference at index: {index}");
                Console.WriteLine($"Total references count: {references.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReferenceCollection: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionReference](../webextensionreference/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


