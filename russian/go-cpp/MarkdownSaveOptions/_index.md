---
title: "Класс MarkdownSaveOptions"
linktitle: "MarkdownSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс MarkdownSaveOptions. Инкапсулирует объект, представляющий markdownsaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Представляет параметры сохранения markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Создаёт параметры для сохранения markdown-документа |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetEncoding](./getencoding/) | Получает и задаёт кодировку по умолчанию. |
| [SetEncoding](./setencoding/) | Получает и задаёт кодировку по умолчанию. |
| [GetFormatStrategy](./getformatstrategy/) | Получает и задаёт стратегию форматирования при экспорте значения ячейки как строки. |
| [SetFormatStrategy](./setformatstrategy/) | Получает и задаёт стратегию форматирования при экспорте значения ячейки как строки. |
| [GetLineSeparator](./getlineseparator/) | Получает и задаёт разделитель строк. |
| [SetLineSeparator](./setlineseparator/) | Получает и задаёт разделитель строк. |
| [GetTableHeaderType](./gettableheadertype/) | Получает и задаёт способ установки заголовка таблицы. |
| [SetTableHeaderType](./settableheadertype/) | Получает и задаёт способ установки заголовка таблицы. |
| [GetSheetSet](./getsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Получите объект ImageOrPrintOptions перед экспортом. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Указывает, сохраняются ли изображения в формате Base64 в Markdown. Значение по умолчанию — true. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Указывает, сохраняются ли изображения в формате Base64 в Markdown. Значение по умолчанию — true. |
| [GetCalculateFormula](./getcalculateformula/) | Указывает, следует ли вычислять формулы перед сохранением файла markdown. |
| [SetCalculateFormula](./setcalculateformula/) | Указывает, следует ли вычислять формулы перед сохранением файла markdown. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Указывает, следует ли экспортировать гиперссылку с использованием определений ссылок вместо встроенного формата. Значение по умолчанию — false. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Указывает, следует ли экспортировать гиперссылку с использованием определений ссылок вместо встроенного формата. Значение по умолчанию — false. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Указывает, включено ли выравнивание столбцов для сгенерированных таблиц Markdown. При включении столбцы выравниваются путем заполнения содержимого ячеек указанным символом (обычно ' ' для пробелов). Установите '\\0', чтобы отключить выравнивание столбцов (по умолчанию). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Указывает, включено ли выравнивание столбцов для сгенерированных таблиц Markdown. При включении столбцы выравниваются путем заполнения содержимого ячеек указанным символом (обычно ' ' для пробелов). Установите '\\0', чтобы отключить выравнивание столбцов (по умолчанию). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Указывает, следует ли рассматривать пустые строки в листе как разделители таблиц при экспорте в Markdown. Значение по умолчанию — false. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Указывает, следует ли рассматривать пустые строки в листе как разделители таблиц при экспорте в Markdown. Значение по умолчанию — false. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | Указывает, как объекты OfficeMath экспортируются в Markdown. Значение по умолчанию — Image. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | Указывает, как объекты OfficeMath экспортируются в Markdown. Значение по умолчанию — Image. |
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
