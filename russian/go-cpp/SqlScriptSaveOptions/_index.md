---
title: "Класс SqlScriptSaveOptions"
linktitle: "SqlScriptSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SqlScriptSaveOptions. Инкапсулирует объект, представляющий sqlscriptsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Представляет параметры сохранения sql.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | Создаёт параметры для сохранения SQL‑файла. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | Проверьте, существует ли имя таблицы перед созданием |
| [SetCheckIfTableExists](./setcheckiftableexists/) | Проверьте, существует ли имя таблицы перед созданием |
| [GetColumnTypeMap](./getcolumntypemap/) | Получает и задаёт карту типов столбцов для разных баз данных. |
| [SetColumnTypeMap](./setcolumntypemap/) | Получает и задаёт карту типов столбцов для разных баз данных. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Проверьте все данные, чтобы определить типы столбцов. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Проверьте все данные, чтобы определить типы столбцов. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Вставьте пустую строку между каждым набором данных. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Вставьте пустую строку между каждым набором данных. |
| [GetSeparator](./getseparator/) | Получает и задаёт символьный разделитель SQL‑скрипта. |
| [SetSeparator](./setseparator/) | Получает и задаёт символьный разделитель SQL‑скрипта. |
| [GetOperatorType](./getoperatortype/) | Получает и задаёт тип оператора SQL. |
| [SetOperatorType](./setoperatortype/) | Получает и задаёт тип оператора SQL. |
| [GetPrimaryKey](./getprimarykey/) | Представляет, какой столбец является первичным ключом таблицы данных. |
| [SetPrimaryKey](./setprimarykey/) | Представляет, какой столбец является первичным ключом таблицы данных. |
| [GetCreateTable](./getcreatetable/) | Указывает, экспортировать ли SQL создания таблицы. |
| [SetCreateTable](./setcreatetable/) | Указывает, экспортировать ли SQL создания таблицы. |
| [GetIdName](./getidname/) | Получает и задаёт имя столбца идентификатора. |
| [SetIdName](./setidname/) | Получает и задаёт имя столбца идентификатора. |
| [GetStartId](./getstartid/) | Получает и задаёт начальный идентификатор. |
| [SetStartId](./setstartid/) | Получает и задаёт начальный идентификатор. |
| [GetTableName](./gettablename/) | Получает и задаёт имя таблицы. |
| [SetTableName](./settablename/) | Получает и задаёт имя таблицы. |
| [GetExportAsString](./getexportasstring/) | Указывает, экспортировать ли все данные как строковое значение. |
| [SetExportAsString](./setexportasstring/) | Указывает, экспортировать ли все данные как строковое значение. |
| [GetSheetIndexes](./getsheetindexes/) | Представляет индексы экспортированных листов. |
| [SetSheetIndexes](./setsheetindexes/) | Представляет индексы экспортированных листов. |
| [GetExportArea](./getexportarea/) | Получает или задаёт диапазон экспорта. |
| [SetExportArea](./setexportarea/) | Получает или задаёт диапазон экспорта. |
| [GetHasHeaderRow](./gethasheaderrow/) | Указывает, содержит ли диапазон строку заголовка. |
| [SetHasHeaderRow](./sethasheaderrow/) | Указывает, содержит ли диапазон строку заголовка. |
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
