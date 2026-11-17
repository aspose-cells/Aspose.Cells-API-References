---
title: "Класс ListObject"
linktitle: "ListObject"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ListObject. Инкапсулирует объект, представляющий listobject в Go."
type: docs
weight: 200
url: /ru/go-cpp/listobject/
---

## ListObject class

Представляет таблицу в листе.

```go

type ListObject struct  {
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
| [GetStartRow](./getstartrow/) | Получает начальную строку диапазона. |
| [GetStartColumn](./getstartcolumn/) | Получает начальный столбец диапазона. |
| [GetEndRow](./getendrow/) | Получает конечную строку диапазона. |
| [GetEndColumn](./getendcolumn/) | Получает конечный столбец диапазона. |
| [GetListColumns](./getlistcolumns/) | Получает список ListColumn этой таблицы. |
| [Resize](./resize/) | Изменить размер диапазона объекта списка. |
| [PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | Поместить значение в ячейку. |
| [PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | Поместить значение в ячейку. |
| [PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | Поместить формулу в ячейку в таблице. |
| [PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | Поместить формулу в ячейку в таблице. |
| [GetShowHeaderRow](./getshowheaderrow/) | Получает и задает, отображает ли эта Table строку заголовка. |
| [SetShowHeaderRow](./setshowheaderrow/) | Получает и задает, отображает ли эта Table строку заголовка. |
| [GetShowTotals](./getshowtotals/) | Получает и задает, отображает ли эта TAble строку итогов. |
| [SetShowTotals](./setshowtotals/) | Получает и задает, отображает ли эта TAble строку итогов. |
| [GetDataRange](./getdatarange/) | Получает диапазон данных Table. |
| [UpdateColumnName](./updatecolumnname/) | Обновляет имена всех столбцов списка в ячейках таблицы. |
| [GetQueryTable](./getquerytable/) | Получает связанный QueryTable. |
| [GetDataSourceType](./getdatasourcetype/) | Получает тип источника данных таблицы. |
| [GetHasAutoFilter](./gethasautofilter/) | Указывает, применён ли автофильтр к этой таблице. |
| [SetHasAutoFilter](./sethasautofilter/) | Указывает, применён ли автофильтр к этой таблице. |
| [RemoveAutoFilter](./removeautofilter/) | Удаляет автофильтр, применённый к этой таблице. |
| [GetAutoFilter](./getautofilter/) | Получает автофильтр этой таблицы. |
| [GetDisplayName](./getdisplayname/) | Получает и задает отображаемое имя таблицы. |
| [SetDisplayName](./setdisplayname/) | Получает и задает отображаемое имя таблицы. |
| [GetComment](./getcomment/) | Получает и задает комментарий таблицы. |
| [SetComment](./setcomment/) | Получает и задает комментарий таблицы. |
| [GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | Указывает, применяется ли стиль к первому столбцу в таблице. |
| [SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | Указывает, применяется ли стиль к первому столбцу в таблице. |
| [GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | Указывает, применяется ли стиль к последнему столбцу в таблице. |
| [SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | Указывает, применяется ли стиль к последнему столбцу в таблице. |
| [GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | Указывает, применяется ли чередование строк к таблице. |
| [SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | Указывает, применяется ли чередование строк к таблице. |
| [GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | Указывает, применяется ли чередование столбцов к таблице. |
| [SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | Указывает, применяется ли чередование столбцов к таблице. |
| [ApplyStyleToRange](./applystyletorange/) | Применить стиль таблицы к диапазону. |
| [ConvertToRange](./converttorange/) | Преобразовать таблицу в диапазон. |
| [ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | Преобразовать таблицу в диапазон. |
| [GetTableStyleType](./gettablestyletype/) | Получает встроенный стиль таблицы. |
| [SetTableStyleType](./settablestyletype/) | Получает встроенный стиль таблицы. |
| [GetTableStyleName](./gettablestylename/) | Получает и задает имя стиля таблицы. |
| [SetTableStyleName](./settablestylename/) | Получает и задает имя стиля таблицы. |
| [GetXmlMap](./getxmlmap/) | Получает XmlMap, используемый для этого списка. |
| [GetAlternativeText](./getalternativetext/) | Получает и задает альтернативный текст. |
| [SetAlternativeText](./setalternativetext/) | Получает и задает альтернативный текст. |
| [GetAlternativeDescription](./getalternativedescription/) | Получает и задает альтернативное описание. |
| [SetAlternativeDescription](./setalternativedescription/) | Получает и задает альтернативное описание. |
