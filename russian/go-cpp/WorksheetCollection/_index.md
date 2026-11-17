---
title: "WorksheetCollection Класс"
linktitle: "WorksheetCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "WorksheetCollection класс. Инкапсулирует объект, представляющий worksheetcollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/worksheetcollection/
---

## WorksheetCollection class

Инкапсулирует коллекцию объектов <see cref="Worksheet"/>.

```go

type WorksheetCollection struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Получает список панелей задач. |
| [GetWebExtensions](./getwebextensions/) | Получает список панелей задач. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Получает список авторов вложенных комментариев. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | Указывает, следует ли обновлять все соединения при открытии файла в MS Excel. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | Указывает, следует ли обновлять все соединения при открытии файла в MS Excel. |
| [CreateRange](./createrange/) | Создает объект Range из адреса диапазона. |
| [CreateUnionRange](./createunionrange/) | Создает объект Range из адреса диапазона. |
| [GetNames](./getnames/) | Получает коллекцию всех объектов Name в электронной таблице. |
| [Get_Int](./get_int/) | Получает элемент Worksheet по указанному индексу. |
| [Get_String](./get_string/) | Получает элемент Worksheet с указанным именем. |
| [GetSheetByCodeName](./getsheetbycodename/) | Получает лист по коду имени. |
| [GetActiveSheetName](./getactivesheetname/) | Представляет имя активного листа при открытии электронной таблицы. |
| [SetActiveSheetName](./setactivesheetname/) | Представляет имя активного листа при открытии электронной таблицы. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Представляет индекс активного листа при открытии электронной таблицы. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Представляет индекс активного листа при открытии электронной таблицы. |
| [SortNames](./sortnames/) | Сортирует определённые имена. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Вставить лист. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Вставить лист. |
| [Add_SheetType](./add_sheettype/) | Добавляет лист в коллекцию. |
| [SwapSheet](./swapsheet/) | Меняет местами два листа. |
| [Add](./add/) | Добавляет лист в коллекцию. |
| [Add_String](./add_string/) | Добавляет лист в коллекцию. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Добавляет функцию надстройки в книгу. |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Добавляет функцию надстройки в книгу. |
| [RemoveAt_String](./removeat_string/) | Удаляет элемент с указанным именем. |
| [RemoveAt_Int](./removeat_int/) | Удаляет элемент по указанному индексу. |
| [Clear](./clear/) | Очистить все листы. |
| [AddCopy_String](./addcopy_string/) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy_Int](./addcopy_int/) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Копировать группу листов. |
| [GetDxfs](./getdxfs/) | Получает главные записи дифференциального форматирования. |
| [GetRangeByName_String](./getrangebyname_string/) | Получает объект Range по предопределённому имени. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Получает Range по предопределённому имени или имени таблицы |
| [GetNamedRanges](./getnamedranges/) | Получает все предопределённые именованные диапазоны в таблице. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Получает все предопределённые именованные диапазоны в таблице. |
| [GetXmlMaps](./getxmlmaps/) | Получает и задаёт XML‑карты в рабочей книге. |
| [SetXmlMaps](./setxmlmaps/) | Получает и задаёт XML‑карты в рабочей книге. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Возвращает коллекцию DocumentProperty, представляющую все встроенные свойства документа электронной таблицы. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Возвращает коллекцию DocumentProperty, представляющую все пользовательские свойства документа электронной таблицы. |
| [GetOleSize](./getolesize/) | Получает и задаёт отображаемый размер, когда файл Workbook используется как объект Ole. |
| [SetOleSize_Object](./setolesize_object/) | Получает и задаёт отображаемый размер, когда файл Workbook используется как объект Ole. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Задаёт отображаемый размер, когда файл Workbook используется как объект Ole. |
| [GetExternalLinks](./getexternallinks/) | Представляет внешние ссылки в рабочей книге. |
| [GetPivotCaches](./getpivotcaches/) | Получает все PivotCache. |
| [GetTableStyles](./gettablestyles/) | Получает объект TableStyles. |
| [ClearPivottables](./clearpivottables/) | Очищает сводные таблицы из таблицы. |
| [GetRevisionLogs](./getrevisionlogs/) | Представляет журналы изменений. |
| [RefreshPivotTables](./refreshpivottables/) | Обновляет все PivotTables в файле Excel. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Обновляет все PivotTables в файле Excel. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Представляет все метки чувствительности. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
