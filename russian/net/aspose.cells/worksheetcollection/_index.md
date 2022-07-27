---
title: WorksheetCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует наборWorksheet./worksheet объекты.
type: docs
weight: 6520
url: /ru/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Инкапсулирует набор[`Worksheet`](../worksheet) объекты.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Представляет индекс активного рабочего листа при открытии электронной таблицы. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Представляет имя активного рабочего листа при открытии электронной таблицы. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Возвращает[`DocumentProperty`](../../aspose.cells.properties/documentproperty)коллекция, которая представляет все встроенные свойства документа электронной таблицы. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Возвращает[`DocumentProperty`](../../aspose.cells.properties/documentproperty) коллекция, которая представляет все настраиваемые свойства документа электронной таблицы. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Получает основные записи дифференциального форматирования. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Представляет внешние ссылки в книге. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Указывает, будут ли обновляться все подключения при открытии файла в MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Получает[`Worksheet`](../worksheet) элемент по указанному индексу. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Получает коллекцию всех объектов Name в электронной таблице. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Получает и задает отображаемый размер, когда файл рабочей книги используется в качестве объекта Ole. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Представляет журналы изменений. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | получает[`TableStyles`](./tablestyles) объект. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Получает список авторов цепочек комментариев. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Получает список областей задач. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Получает список областей задач. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Получает и задает карты XML в книге. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Добавляет рабочий лист в коллекцию. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Добавляет рабочий лист в коллекцию. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Добавляет рабочий лист в коллекцию. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Очистить все листы. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Удаляет сводные таблицы из электронной таблицы. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Создает[`Range`](../range) объект с адреса диапазона. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Создает[`Range`](../range) объект с адреса диапазона. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Получает все предопределенные именованные диапазоны в электронной таблице. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Получает все предопределенные именованные диапазоны в электронной таблице. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Получает объект Range по заданному имени. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | получает[`Range`](../range) по заданному имени или имени таблицы |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Получает рабочий лист по кодовому имени. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Вставить рабочий лист. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Вставить рабочий лист. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Обновляет все сводные таблицы в WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Добавляет функцию надстройки в книгу |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Добавляет функцию надстройки в книгу |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Удаляет элемент по указанному индексу. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Удаляет элемент с указанным именем. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Устанавливает отображаемый размер, когда файл рабочей книги используется в качестве объекта Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Сортирует определенные имена. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Меняет местами два листа. |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Добавить рабочий лист
sheets.Add();

//Изменить имя рабочего листа
sheets[0].Name = "First Sheet";

//Установим активный лист на второй рабочий лист
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Добавить рабочий лист
sheets.Add()

'Изменить имя рабочего листа
sheets(0).Name = "First Sheet"

'Установите активный лист на второй рабочий лист
sheets.ActiveSheetIndex = 1
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
