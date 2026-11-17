---
title: "Класс AutoFilter"
linktitle: "AutoFilter"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс AutoFilter. Инкапсулирует объект, представляющий автофильтр в Go."
type: docs
weight: 200
url: /ru/go-cpp/autofilter/
---

## AutoFilter class

Представляет автофильтрацию для указанного листа.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Получает сортировщик данных. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Устанавливает диапазон, к которому применяется указанный AutoFilter. |
| [GetCellArea](./getcellarea/) | Получает CellArea, к которому применяется данный AutoFilter. |
| [GetCellArea_Bool](./getcellarea_bool/) | Получает Aspose.Cells.CellArea, к которому применяется указанный AutoFilter. |
| [GetRange](./getrange/) | Представляет диапазон, к которому применяется указанный AutoFilter. |
| [SetRange_String](./setrange_string/) | Представляет диапазон, к которому применяется указанный AutoFilter. |
| [AddFilter](./addfilter/) | Добавляет фильтр для столбца фильтра. |
| [AddDateFilter](./adddatefilter/) | Добавляет фильтр по дате. |
| [RemoveDateFilter](./removedatefilter/) | Удаляет фильтр по дате. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Удаляет фильтр для столбца фильтра. |
| [Filter](./filter/) | Фильтрует список с указанными критериями. |
| [FilterTop10](./filtertop10/) | Отфильтровать 10 лучших элементов в списке |
| [Dynamic_Filter](./dynamic_filter/) | Добавляет динамический фильтр. |
| [AddFontColorFilter](./addfontcolorfilter/) | Добавляет фильтр по цвету шрифта. |
| [AddFillColorFilter](./addfillcolorfilter/) | Добавляет фильтр по цвету заливки. |
| [AddIconFilter](./addiconfilter/) | Добавляет фильтр по значку. |
| [MatchBlanks](./matchblanks/) | Соответствует всем пустым ячейкам в списке. |
| [MatchNonBlanks](./matchnonblanks/) | Соответствует всем непустым ячейкам в списке. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Фильтрует список с пользовательским критерием. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Фильтрует список с использованием пользовательских критериев. |
| [ShowAll](./showall/) | Отобразить все скрытые строки. |
| [RemoveFilter_Int](./removefilter_int/) | Удалить конкретный фильтр. |
| [Refresh](./refresh/) | Обновить автофильтры, чтобы скрыть или отобразить строки. |
| [Refresh_Bool](./refresh_bool/) | Получает индексы всех скрытых строк. |
| [GetShowFilterButton](./getshowfilterbutton/) | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [SetShowFilterButton](./setshowfilterbutton/) | Указывает, видна ли кнопка AutoFilter для этого столбца. |
| [GetFilterColumns](./getfiltercolumns/) | Получает коллекцию столбцов фильтра. |
