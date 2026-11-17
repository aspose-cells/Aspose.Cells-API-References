---
title: "Класс TxtSaveOptions"
linktitle: "TxtSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс TxtSaveOptions. Инкапсулирует объект, представляющий txtsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Представляет параметры сохранения для формата csv/разделённого табуляцией/других текстовых форматов.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Создаёт параметры сохранения текстового файла. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Создаёт параметры сохранения текстового файла. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetSeparator](./getseparator/) | Получает и задаёт символ‑разделитель текстового файла. |
| [SetSeparator](./setseparator/) | Получает и задаёт символ‑разделитель текстового файла. |
| [GetSeparatorString](./getseparatorstring/) | Получает и задаёт строковое значение в качестве разделителя. |
| [SetSeparatorString](./setseparatorstring/) | Получает и задаёт строковое значение в качестве разделителя. |
| [GetEncoding](./getencoding/) | Получает и задаёт кодировку по умолчанию. |
| [SetEncoding](./setencoding/) | Получает и задаёт кодировку по умолчанию. |
| [GetQuoteType](./getquotetype/) | Получает или задаёт способ кавычек значений в экспортируемом текстовом файле. |
| [SetQuoteType](./setquotetype/) | Получает или задаёт способ кавычек значений в экспортируемом текстовом файле. |
| [GetFormatStrategy](./getformatstrategy/) | Получает и задаёт стратегию форматирования при экспорте значения ячейки как строки. |
| [SetFormatStrategy](./setformatstrategy/) | Получает и задаёт стратегию форматирования при экспорте значения ячейки как строки. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Указывает, следует ли обрезать ведущие пустые строки и столбцы, как делает MS Excel. По умолчанию true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Указывает, следует ли обрезать ведущие пустые строки и столбцы, как делает MS Excel. По умолчанию true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Указывает, следует ли обрезать завершающие пустые ячейки в строке. По умолчанию false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Указывает, следует ли обрезать завершающие пустые ячейки в строке. По умолчанию false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию — false, поэтому содержимое пустой строки будет пустым. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию — false, поэтому содержимое пустой строки будет пустым. |
| [GetExportArea](./getexportarea/) | Диапазон ячеек для экспорта. |
| [SetExportArea](./setexportarea/) | Диапазон ячеек для экспорта. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Указывает, следует ли экспортировать одинарную кавычку как часть значения ячейки, когда для неё установлен Style.QuotePrefix = true. По умолчанию false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Указывает, следует ли экспортировать одинарную кавычку как часть значения ячейки, когда для неё установлен Style.QuotePrefix = true. По умолчанию false. |
| [GetExportAllSheets](./getexportallsheets/) | Указывает, следует ли экспортировать все листы в текстовый файл. Если false, экспортируется только активный лист, как в MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | Указывает, следует ли экспортировать все листы в текстовый файл. Если false, экспортируется только активный лист, как в MS Excel. |
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
