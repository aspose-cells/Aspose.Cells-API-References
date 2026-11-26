---
title: "Класс GridHtmlSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions. Представляет параметры сохранения html‑файла"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Представляет параметры сохранения HTML‑файла.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | Создаёт параметры для сохранения HTML‑файла. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | Создаёт параметры для сохранения HTM‑файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток HTML. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Укажите префикс URL вложенных файлов, например изображений, в HTML‑файле. Только при сохранении в поток HTML. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | Папка кэшированных файлов используется для хранения некоторых больших данных.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | Укажите имя шрифта по умолчанию для экспорта HTML; этот шрифт будет использоваться, если шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells использует универсальный шрифт той же семейства, что и оригинальный шрифт. Значение по умолчанию — null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Указывает, экспортировать ли всю книгу в html‑файл. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Получает или задаёт экспортируемую CellArea текущего активного листа Worksheet. Если задать этот атрибут, область печати текущего активного листа Worksheet будет опущена. При сохранении файла в html будет экспортирована только указанная область. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Указывает, экспортировать ли линии сетки.Значение по умолчанию — false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Указывает, экспортировать ли заголовки при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, оставьте значение по умолчанию. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Указывает, экспортировать ли скрытое содержимое листа.Значение по умолчанию — true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Указывает, экспортировать ли комментарии при сохранении файла в HTML, значение по умолчанию — false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | Указывает, использовать ли полные пути в ссылках в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | Заголовок HTML‑страницы. Только при сохранении в поток HTML. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Разбирать html‑тег в ячейке, например , как значение ячейки или как html‑тег, по умолчанию true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Указывает, предпочтителен ли html или mht файл для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Указывает, следует ли обновлять кэш данных диаграмм (Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Получает формат сохраняемого файла.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Указывает, следует ли сортировать определённые имена перед сохранением файла.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Указывает, следует ли проверять объединённые ячейки перед сохранением файла.(Наследовано от [`GridSaveOptions`](../gridsaveoptions/).) |

### См. также

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


