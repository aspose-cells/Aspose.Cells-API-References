---
title: GridHtmlSaveOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры сохранения HTML-файла.
type: docs
weight: 250
url: /ru/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Представляет параметры сохранения HTML-файла.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Создает параметры для сохранения html-файла. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | Создает параметры для сохранения htm-файла. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | Каталог, в который будут сохраняться вложенные файлы. Только для сохранения в поток html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | Укажите префикс URL вложенных файлов, таких как изображение в файле html. Только для сохранения в поток html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | Папка с кэшированными файлами используется для хранения больших данных. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Сделайте рабочую книгу пустой после сохранения файла. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Укажите имя шрифта по умолчанию для экспорта html, шрифт по умолчанию будет использоваться, когда шрифт стиля не существует, Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт, который имеет то же семейство, что и исходный шрифт, значение по умолчанию равно null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Если не задано, используйте Encoding.UTF8 в качестве типа кодирования по умолчанию. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Указывает, экспортируется ли вся книга в файл html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Получает или задает экспортируемую CellArea текущего активного рабочего листа. Если вы установите этот атрибут, область печати текущего активного рабочего листа будет опущена. Только указанная область будет экспортирована при сохранении файла в html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Указывает, экспортируются ли линии сетки. Значение по умолчанию — false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Указывает, экспортируются ли заголовки при сохранении файла в формате html. Значение по умолчанию — false. Если вы хотите импортировать файл html в Excel, оставьте значение по умолчанию. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Указывает, экспортируется ли скрытое содержимое рабочего листа. Значение по умолчанию — true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Указывает, экспортируется ли только область печати в html-файл. Значение по умолчанию — false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Указывает, следует ли экспортировать одну вкладку, когда файл содержит только один рабочий лист. Значение по умолчанию — false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Указывает, что при экспорте комментариев при сохранении файла в html значение по умолчанию равно false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Указывает, используется ли полный путь в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | Заголовок html-страницы. Только для сохранения в html-поток. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | Разобрать HTML-тег в ячейке, например , как значение ячейки или как HTML-тег, по умолчанию true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | Указывает, является ли файл html или mht предпочтительным для презентации. Значение по умолчанию — false. Если вы хотите получить более красивую презентацию, установите значение true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Указывает, нужно ли обновлять кэш диаграммы data |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Получает формат файла сохранения. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Указывает, выполняется ли сортировка определенных имен перед сохранением файла. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Указывает, следует ли проверять объединенные ячейки перед сохранением файла. |

### Смотрите также

* class [GridSaveOptions](../gridsaveoptions)
* пространство имен [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* сборка [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
