---
title: "Класс SpreadsheetML2003SaveOptions"
linktitle: "SpreadsheetML2003SaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SpreadsheetML2003SaveOptions. Инкапсулирует объект, представляющий spreadsheetml2003saveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

Представляет параметры сохранения файла Excel 2003 spreadml.

```go

type SpreadsheetML2003SaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSpreadsheetML2003SaveOptions](./newspreadsheetml2003saveoptions/) | Создаёт параметры для сохранения файла Excel 2003 spreadml. |
| [NewSpreadsheetML2003SaveOptions_SaveOptions](./newspreadsheetml2003saveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [IsIndentedFormatting](./isindentedformatting/) | Заставляет дочерние элементы быть с отступом. |
| [SetIsIndentedFormatting](./setisindentedformatting/) | Заставляет дочерние элементы быть с отступом. |
| [GetLimitAsXls](./getlimitasxls/) | Ограничение для xls: максимальный индекс строки — 65535, а максимальный индекс столбца — 255. |
| [SetLimitAsXls](./setlimitasxls/) | Ограничение для xls: максимальный индекс строки — 65535, а максимальный индекс столбца — 255. |
| [GetExportColumnIndexOfCell](./getexportcolumnindexofcell/) | Значение по умолчанию — false, это означает, что индекс столбца будет игнорироваться, если ячейка смежна с предыдущей ячейкой. |
| [SetExportColumnIndexOfCell](./setexportcolumnindexofcell/) | Значение по умолчанию — false, это означает, что индекс столбца будет игнорироваться, если ячейка смежна с предыдущей ячейкой. |
| [GetSaveFormat](./getsaveformat/) | Получает формат сохраняемого файла. |
| [GetClearData](./getcleardata/) | Очищает книгу после сохранения файла. |
| [SetClearData](./setcleardata/) | Очищает книгу после сохранения файла. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Указывает, следует ли проверять объединённые ячейки перед сохранением файла. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Указывает, следует ли проверять объединённые ячейки перед сохранением файла. |
| [GetMergeAreas](./getmergeareas/) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [SetMergeAreas](./setmergeareas/) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [GetCreateDirectory](./getcreatedirectory/) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [SetCreateDirectory](./setcreatedirectory/) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [GetSortNames](./getsortnames/) | Указывает, следует ли сортировать определённые имена перед сохранением файла. |
| [SetSortNames](./setsortnames/) | Указывает, следует ли сортировать определённые имена перед сохранением файла. |
| [GetSortExternalNames](./getsortexternalnames/) | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла. |
| [SetSortExternalNames](./setsortexternalnames/) | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Указывает, следует ли кэшировать последние данные диаграммы. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Указывает, следует ли кэшировать последние данные диаграммы. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Проверять ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если ввести значение длиной более 32 КБ, оно будет усечено. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Проверять ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если ввести значение длиной более 32 КБ, оно будет усечено. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Указывает, следует ли обновлять настройки SmartArt. Значение по умолчанию — false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Указывает, следует ли обновлять настройки SmartArt. Значение по умолчанию — false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true. |
