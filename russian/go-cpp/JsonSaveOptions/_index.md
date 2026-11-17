---
title: "Класс JsonSaveOptions"
linktitle: "JsonSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс JsonSaveOptions. Инкапсулирует объект, представляющий jsonsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Представляет параметры сохранения рабочей книги в виде JSON‑файла.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | Создаёт параметры для сохранения JSON‑файла. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetExportStylePool](./getexportstylepool/) | Указывает, экспортировать стили совместно или индивидуально для каждой ячейки. |
| [SetExportStylePool](./setexportstylepool/) | Указывает, экспортировать стили совместно или индивидуально для каждой ячейки. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | Представляет тип экспорта гиперссылки в JSON. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | Представляет тип экспорта гиперссылки в JSON. |
| [GetSkipEmptyRows](./getskipemptyrows/) | Указывает, пропускать ли пустые строки. |
| [SetSkipEmptyRows](./setskipemptyrows/) | Указывает, пропускать ли пустые строки. |
| [GetSheetIndexes](./getsheetindexes/) | Представляет индексы экспортированных листов. |
| [SetSheetIndexes](./setsheetindexes/) | Представляет индексы экспортированных листов. |
| [GetSchemas](./getschemas/) | Исходная JSON‑схема каждого листа. |
| [SetSchemas](./setschemas/) | Исходная JSON‑схема каждого листа. |
| [GetExportArea](./getexportarea/) | Получает или задаёт диапазон экспорта. |
| [SetExportArea](./setexportarea/) | Получает или задаёт диапазон экспорта. |
| [GetHasHeaderRow](./gethasheaderrow/) | Указывает, содержит ли диапазон строку заголовка. |
| [SetHasHeaderRow](./sethasheaderrow/) | Указывает, содержит ли диапазон строку заголовка. |
| [GetExportAsString](./getexportasstring/) | Экспортирует строковые значения ячеек в JSON. |
| [SetExportAsString](./setexportasstring/) | Экспортирует строковые значения ячеек в JSON. |
| [GetIndent](./getindent/) | Указывает отступ. |
| [SetIndent](./setindent/) | Указывает отступ. |
| [GetExportNestedStructure](./getexportnestedstructure/) | Экспортировано как иерархическая структура JSON родитель‑дочерний. |
| [SetExportNestedStructure](./setexportnestedstructure/) | Экспортировано как иерархическая структура JSON родитель‑дочерний. |
| [GetExportEmptyCells](./getexportemptycells/) | Указывает, экспортировать ли пустые ячейки как null. |
| [SetExportEmptyCells](./setexportemptycells/) | Указывает, экспортировать ли пустые ячейки как null. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Указывает, всегда ли экспортировать Excel в JSON как объект, даже если в файле только один лист. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Указывает, всегда ли экспортировать Excel в JSON как объект, даже если в файле только один лист. |
| [GetToExcelStruct](./gettoexcelstruct/) | Указывает, следует ли преобразовать в структуру json Excel‑файла. |
| [SetToExcelStruct](./settoexcelstruct/) | Указывает, следует ли преобразовать в структуру json Excel‑файла. |
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
