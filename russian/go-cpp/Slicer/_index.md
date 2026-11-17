---
title: "Класс Slicer"
linktitle: "Slicer"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Slicer. Инкапсулирует объект, представляющий слайсер в Go."
type: docs
weight: 200
url: /ru/go-cpp/slicer/
---

## Slicer class

краткое описание Slicer View

```go

type Slicer struct  {
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
| [GetSortOrderType](./getsortordertype/) | Указывает тип сортировки элементов. |
| [SetSortOrderType](./setsortordertype/) | Указывает тип сортировки элементов. |
| [GetShowMissing](./getshowmissing/) | Указывает, следует ли показывать элементы, удалённые из источника данных. |
| [SetShowMissing](./setshowmissing/) | Указывает, следует ли показывать элементы, удалённые из источника данных. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Указывает, следует ли показывать элементы, удалённые из источника данных. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Указывает, следует ли показывать элементы, удалённые из источника данных. |
| [GetShowAllItems](./getshowallitems/) | Указывает, следует ли показывать все элементы, даже если данных нет или они удалены. Значение по умолчанию — true; |
| [SetShowAllItems](./setshowallitems/) | Указывает, следует ли показывать все элементы, даже если данных нет или они удалены. Значение по умолчанию — true; |
| [AddPivotConnection](./addpivotconnection/) | Добавляет соединение PivotTable. |
| [RemovePivotConnection](./removepivotconnection/) | Удаляет соединение PivotTable. |
| [GetLockedPosition](./getlockedposition/) | Указывает, может ли указанный слайсер перемещаться или изменять размер с помощью пользовательского интерфейса. |
| [SetLockedPosition](./setlockedposition/) | Указывает, может ли указанный слайсер перемещаться или изменять размер с помощью пользовательского интерфейса. |
| [Refresh](./refresh/) | Обновление элементов слайсера из связанных сводных таблиц. |
| [GetShape](./getshape/) | Возвращает объект Shape, связанный с указанным слайсером. Только для чтения. |
| [GetSlicerCache](./getslicercache/) | Возвращает объект SlicerCache, связанный с слайсером. Только для чтения. |
| [GetWorksheet](./getworksheet/) | Возвращает объект Worksheet, содержащий этот слайсер. Только для чтения. |
| [GetStyleType](./getstyletype/) | Укажите тип встроенного стиля слайсера. Тип по умолчанию — SlicerStyleLight1. |
| [SetStyleType](./setstyletype/) | Укажите тип встроенного стиля слайсера. Тип по умолчанию — SlicerStyleLight1. |
| [GetName](./getname/) | Возвращает или задаёт имя указанного слайсера |
| [SetName](./setname/) | Возвращает или задаёт имя указанного слайсера |
| [GetCaption](./getcaption/) | Возвращает или задаёт подпись указанного слайсера. |
| [SetCaption](./setcaption/) | Возвращает или задаёт подпись указанного слайсера. |
| [GetFirstItemIndex](./getfirstitemindex/) | Указывает нулевой индекс первого элемента слайсера. |
| [SetFirstItemIndex](./setfirstitemindex/) | Указывает нулевой индекс первого элемента слайсера. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | Удалить выбранные метки фильтра. |
| [ClearFilter](./clearfilter/) | Удалить фильтры |
| [GetShowCaption](./getshowcaption/) | Указывает, виден ли заголовок слайсера. Значение по умолчанию — true |
| [SetShowCaption](./setshowcaption/) | Указывает, виден ли заголовок слайсера. Значение по умолчанию — true |
| [GetNumberOfColumns](./getnumberofcolumns/) | Возвращает или задаёт количество столбцов в слайсере. Значение по умолчанию — 1. |
| [SetNumberOfColumns](./setnumberofcolumns/) | Возвращает или задаёт количество столбцов в слайсере. Значение по умолчанию — 1. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Получает или задаёт ширину каждого столбца в слайсере в пикселях. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Получает или задаёт ширину каждого столбца в слайсере в пикселях. |
| [GetColumnWidth](./getcolumnwidth/) | Возвращает или задаёт ширину каждого столбца в слайсере в пунктах. |
| [SetColumnWidth](./setcolumnwidth/) | Возвращает или задаёт ширину каждого столбца в слайсере в пунктах. |
| [GetRowHeightPixel](./getrowheightpixel/) | Возвращает или задаёт высоту каждой строки в указанном слайсере в пикселях. |
| [SetRowHeightPixel](./setrowheightpixel/) | Возвращает или задаёт высоту каждой строки в указанном слайсере в пикселях. |
| [GetRowHeight](./getrowheight/) | Возвращает или задаёт высоту каждой строки в указанном слайсере в пунктах. |
| [SetRowHeight](./setrowheight/) | Возвращает или задаёт высоту каждой строки в указанном слайсере в пунктах. |
