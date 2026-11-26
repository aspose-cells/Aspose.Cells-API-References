---
title: "Класс WorksheetCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WorksheetCollection. Инкапсулирует коллекцию объектов Worksheet"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Инкапсулирует коллекцию объектов [`Worksheet`](../worksheet/).

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Представляет индекс активного листа при открытии таблицы. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Представляет имя активного листа при открытии таблицы. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Возвращает коллекцию [`DocumentProperty`](../../aspose.cells.properties/documentproperty/), представляющую все встроенные свойства документа таблицы. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Возвращает коллекцию [`DocumentProperty`](../../aspose.cells.properties/documentproperty/), представляющую все пользовательские свойства документа таблицы. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Получает записи главного дифференциального форматирования. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Представляет внешние ссылки в книге. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | Указывает, следует ли обновлять все соединения при открытии файла в MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Получает элемент [`Worksheet`](../worksheet/) по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Получает коллекцию всех объектов Name в таблице. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Получает и задает отображаемый размер, когда файл Workbook используется как объект OLE. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Получает все [`PivotCache`](../../aspose.cells.pivot/pivotcache/). |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Представляет журналы ревизий. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Представляет все метки чувствительности. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | Получает объект [`TableStyles`](./tablestyles/). |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | Получает список авторов ветвящихся комментариев. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Получает список панелей задач. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Получает список панелей задач. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Получает и задает XML‑карты в книге. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Добавляет лист в коллекцию. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Добавляет лист в коллекцию. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Добавляет лист в коллекцию. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Копировать группу листов. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Очистить все листы. (2 метода) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Удаляет сводные таблицы из электронной таблицы. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Создает объект [`Range`](../range/) из адреса диапазона. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Создает объект [`Range`](../range/) из адреса диапазона. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Получает все предопределённые именованные диапазоны в электронной таблице. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Получает все предопределённые именованные диапазоны в электронной таблице. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Получает объект Range по предопределённому имени. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Получает [`Range`](../range/) по предопределённому имени или имени таблицы |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Получает лист по коду имени. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Вставить лист. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Вставить лист. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Устарело.**) Обновить все сводные таблицы и диаграммы с источником сводных данных. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Обновляет все сводные таблицы в файле Excel. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Обновляет все сводные таблицы в файле Excel. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Добавляет функцию надстройки в книгу |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Добавляет функцию надстройки в книгу |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Удаляет элемент по указанному индексу. (2 метода) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Удаляет элемент по указанному имени. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Устанавливает отображаемый размер, когда файл книги используется как объект OLE. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Сортирует определённые имена. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | Меняет местами два листа. |

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Добавить новый лист в коллекцию
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Получить существующий лист по индексу
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Получить существующий лист по имени
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Установить активный лист
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Установить имя активного листа
            worksheets.ActiveSheetName = "NewSheet";

            // Обновить все сводные таблицы в книге
            worksheets.RefreshAll();

            // Очистить все сводные таблицы из книги
            worksheets.ClearPivottables();

            // Сохраните книгу
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


