---
title: "Класс OoxmlSaveOptions"
linktitle: "OoxmlSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс OoxmlSaveOptions. Инкапсулирует объект, представляющий ooxmlsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Представляет параметры сохранения файла Office Open XML.

```go

type OoxmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewOoxmlSaveOptions](./newooxmlsaveoptions/) | Создаёт параметры для сохранения файла Office Open XML. |
| [NewOoxmlSaveOptions_SaveFormat](./newooxmlsaveoptions_saveformat/) | Создаёт параметры для сохранения файла Office Open XML. |
| [NewOoxmlSaveOptions_SaveOptions](./newooxmlsaveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetAsFlatOpc](./getasflatopc/) | Указывает, следует ли сохранять как плоский OPC‑файл, который может быть сгенерирован Open XML SDK. |
| [SetAsFlatOpc](./setasflatopc/) | Указывает, следует ли сохранять как плоский OPC‑файл, который может быть сгенерирован Open XML SDK. |
| [GetExportCellName](./getexportcellname/) | Указывает, экспортировать ли имя ячейки в файл Excel2007 .xlsx (.xlsm, .xltx, .xltm). Если файл может быть доступен SQL Server DTS, это значение должно быть true. Установка значения в false значительно повышает производительность и уменьшает размер файла при создании больших файлов. Значение по умолчанию — true. |
| [SetExportCellName](./setexportcellname/) | Указывает, экспортировать ли имя ячейки в файл Excel2007 .xlsx (.xlsm, .xltx, .xltm). Если файл может быть доступен SQL Server DTS, это значение должно быть true. Установка значения в false значительно повышает производительность и уменьшает размер файла при создании больших файлов. Значение по умолчанию — true. |
| [GetUpdateZoom](./getupdatezoom/) | Указывает, обновлять ли коэффициент масштабирования перед сохранением файла, если свойства PageSetup.FitToPagesWide и PageSetup.FitToPagesTall управляют масштабированием листа. |
| [SetUpdateZoom](./setupdatezoom/) | Указывает, обновлять ли коэффициент масштабирования перед сохранением файла, если свойства PageSetup.FitToPagesWide и PageSetup.FitToPagesTall управляют масштабированием листа. |
| [GetEnableZip64](./getenablezip64/) | Использовать расширения ZIP64 при записи zip‑архивов, при необходимости. |
| [SetEnableZip64](./setenablezip64/) | Использовать расширения ZIP64 при записи zip‑архивов, при необходимости. |
| [GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | Указывает, встраивать ли файлы Ooxml объекта OleObject как ole‑объект. |
| [SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | Указывает, встраивать ли файлы Ooxml объекта OleObject как ole‑объект. |
| [GetCompressionType](./getcompressiontype/) | Получает и задаёт тип сжатия для файла ooxml. |
| [SetCompressionType](./setcompressiontype/) | Получает и задаёт тип сжатия для файла ooxml. |
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
