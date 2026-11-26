---
title: "Класс HtmlTableLoadOptionCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HtmlTableLoadOptionCollection. Представляет параметры таблицы при импорте HTML"
type: docs
url: /ru/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

Представляет параметры таблицы при импорте HTML.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Получает элемент [`HtmlTableLoadOption`](../htmltableloadoption/) по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | Указывает, следует ли генерировать объекты списка из импортированных таблиц. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) Добавляет один HtmlTableLoadOption в эту коллекцию. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Добавьте HtmlTableLoadOption в список. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Добавьте HtmlTableLoadOption в список. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Добавьте HtmlTableLoadOption в список. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Добавьте HtmlTableLoadOption в список. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Добавьте HtmlTableLoadOption в список. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Добавьте HtmlTableLoadOption в список. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Добавляет один HtmlTableLoadOption в эту коллекцию. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Получите доступ к экземпляру HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Установите свойство TableToListObject
            tableLoadOptions.TableToListObject = true;

            // Добавьте новый HtmlTableLoadOption по индексу таблицы
            int index1 = tableLoadOptions.Add(0);

            // Добавьте новый HtmlTableLoadOption по идентификатору таблицы
            int index2 = tableLoadOptions.Add("tableId");

            // Добавьте новый HtmlTableLoadOption по индексу таблицы и индексу целевого листа
            int index3 = tableLoadOptions.Add(1, 1);

            // Добавьте новый HtmlTableLoadOption по идентификатору таблицы и индексу целевого листа
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Добавьте новый HtmlTableLoadOption по индексу таблицы, индексу целевого листа и индексу исходного листа
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Добавьте новый HtmlTableLoadOption по идентификатору таблицы, индексу целевого листа и индексу исходного листа
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Обратитесь к HtmlTableLoadOption по определённому индексу
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Установите свойства HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Загрузите HTML‑файл в рабочую книгу, используя параметры загрузки
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Сохраните книгу
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


