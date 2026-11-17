---
title: "Класс XmlSaveOptions"
linktitle: "XmlSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс XmlSaveOptions. Инкапсулирует объект, представляющий xmlsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

Представляет параметры сохранения рабочей книги в виде xml-файла.

```go

type XmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewXmlSaveOptions](./newxmlsaveoptions/) | Создаёт параметры для сохранения xml‑файла. |
| [NewXmlSaveOptions_SaveOptions](./newxmlsaveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetSheetIndexes](./getsheetindexes/) | Представляет индексы экспортированных листов. |
| [SetSheetIndexes](./setsheetindexes/) | Представляет индексы экспортированных листов. |
| [GetExportArea](./getexportarea/) | Получает или задаёт диапазон экспорта. |
| [SetExportArea](./setexportarea/) | Получает или задаёт диапазон экспорта. |
| [GetHasHeaderRow](./gethasheaderrow/) | Указывает, содержит ли диапазон строку заголовка. |
| [SetHasHeaderRow](./sethasheaderrow/) | Указывает, содержит ли диапазон строку заголовка. |
| [GetXmlMapName](./getxmlmapname/) | Указывает, экспортировать ли xml‑карту в файл. |
| [SetXmlMapName](./setxmlmapname/) | Указывает, экспортировать ли xml‑карту в файл. |
| [GetSheetNameAsElementName](./getsheetnameaselementname/) | Указывает, экспортировать ли имя листа как имя элемента. |
| [SetSheetNameAsElementName](./setsheetnameaselementname/) | Указывает, экспортировать ли имя листа как имя элемента. |
| [GetDataAsAttribute](./getdataasattribute/) | Указывает, экспортируются ли данные как атрибуты элемента. |
| [SetDataAsAttribute](./setdataasattribute/) | Указывает, экспортируются ли данные как атрибуты элемента. |
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
