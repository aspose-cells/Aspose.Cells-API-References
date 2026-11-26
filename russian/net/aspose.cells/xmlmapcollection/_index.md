---
title: "Класс XmlMapCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.XmlMapCollection. Коллекция объектов XmlMap, представляющих информацию XmlMap"
type: docs
url: /ru/net/aspose.cells/xmlmapcollection/
---
## XmlMapCollection class

Коллекция объектов [`XmlMap`](../xmlmap/), представляющих информацию XmlMap.

```csharp
public class XmlMapCollection : CollectionBase<XmlMap>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/xmlmapcollection/item/) { get; } | Получает xml‑map по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/xmlmapcollection/add/)(string) | Добавить [`XmlMap`](../xmlmap/) по URL/пути XML/XSD‑файла. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [Clear](../../aspose.cells/xmlmapcollection/clear/#clear)() | Удаляет все XmlMap. (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(XmlMap) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, XmlMap[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;XmlMap&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;XmlMap&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlMapCollectionDemo
    {
        public static void XmlMapCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к XmlMapCollection из рабочей книги
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Добавить новый XmlMap в коллекцию
            int xmlMapIndex = xmlMaps.Add("sample.xml");

            // Получить доступ к только что добавленному XmlMap
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Отобразить количество XmlMap в коллекции
            Console.WriteLine("Number of XmlMaps: " + xmlMaps.Count);

            // Установить ёмкость XmlMapCollection
            xmlMaps.Capacity = 10;

            // Очистить все XmlMap из коллекции
            xmlMaps.Clear();

            // Сохраните книгу
            workbook.Save("XmlMapCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [XmlMap](../xmlmap/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


