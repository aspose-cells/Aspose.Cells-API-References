---
title: "ImportTableOptions Класс"
linktitle: "ImportTableOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "ImportTableOptions class. Инкапсулирует объект, представляющий importtableoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/importtableoptions/
---

## ImportTableOptions class

Представляет параметры импорта данных в ячейки.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | Создает параметры импорта по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetConvertGridStyle](./getconvertgridstyle/) | Указывает, следует ли применять стиль представления сетки к ячейкам. |
| [SetConvertGridStyle](./setconvertgridstyle/) | Указывает, следует ли применять стиль представления сетки к ячейкам. |
| [GetConvertNumericData](./getconvertnumericdata/) | Получает или задает значение, указывающее, следует ли преобразовать строковое значение в числовое или дату. |
| [SetConvertNumericData](./setconvertnumericdata/) | Получает или задает значение, указывающее, следует ли преобразовать строковое значение в числовое или дату. |
| [GetInsertRows](./getinsertrows/) | Указывает, следует ли добавлять новые строки при импорте записей данных. |
| [SetInsertRows](./setinsertrows/) | Указывает, следует ли добавлять новые строки при импорте записей данных. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | Указывает, следует ли смещать первую строку вниз при вставке строк. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | Указывает, следует ли смещать первую строку вниз при вставке строк. |
| [IsFieldNameShown](./isfieldnameshown/) | Указывает, следует ли импортировать имя поля. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | Указывает, следует ли импортировать имя поля. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Указывает, следует ли экспортировать подпись как имя поля |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Указывает, следует ли экспортировать подпись как имя поля |
| [GetDateFormat](./getdateformat/) | Получает или задает строку формата даты для ячеек с импортированными значениями datetime. |
| [SetDateFormat](./setdateformat/) | Получает или задает строку формата даты для ячеек с импортированными значениями datetime. |
| [GetNumberFormats](./getnumberformats/) | Получает или задает числовые форматы |
| [SetNumberFormats](./setnumberformats/) | Получает или задает числовые форматы |
| [GetStyles](./getstyles/) | Получает и задает стили для каждого столбца таблицы. |
| [SetStyles](./setstyles/) | Получает и задает стили для каждого столбца таблицы. |
| [GetIsFormulas](./getisformulas/) | Указывает, являются ли данные формулами. |
| [SetIsFormulas](./setisformulas/) | Указывает, являются ли данные формулами. |
| [GetTotalRows](./gettotalrows/) | Получает или задает общее количество строк для импорта из источника данных. -1 означает все строки данного источника данных. |
| [SetTotalRows](./settotalrows/) | Получает или задает общее количество строк для импорта из источника данных. -1 означает все строки данного источника данных. |
| [GetTotalColumns](./gettotalcolumns/) | Получает или задает общее количество столбцов для импорта из источника данных. -1 означает все строки данного источника данных. |
| [SetTotalColumns](./settotalcolumns/) | Получает или задает общее количество столбцов для импорта из источника данных. -1 означает все строки данного источника данных. |
| [GetColumnIndexes](./getcolumnindexes/) | Получает или задает столбцы (нумерация с нуля) для импорта из источника данных. null означает, что следует импортировать все столбцы. |
| [SetColumnIndexes](./setcolumnindexes/) | Получает или задает столбцы (нумерация с нуля) для импорта из источника данных. null означает, что следует импортировать все столбцы. |
| [GetDefaultValues](./getdefaultvalues/) | Значение по умолчанию для значения в таблице — null. |
| [SetDefaultValues](./setdefaultvalues/) | Значение по умолчанию для значения в таблице — null. |
| [IsHtmlString](./ishtmlstring/) | Указывает, содержит ли значение HTML‑теги. |
| [SetIsHtmlString](./setishtmlstring/) | Указывает, содержит ли значение HTML‑теги. |
| [GetCheckMergedCells](./getcheckmergedcells/) | Указывает, проверять ли объединённые ячейки. |
| [SetCheckMergedCells](./setcheckmergedcells/) | Указывает, проверять ли объединённые ячейки. |
