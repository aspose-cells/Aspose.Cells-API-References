---
title: "Класс EbookSaveOptions"
linktitle: "EbookSaveOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс EbookSaveOptions. Инкапсулирует объект, представляющий ebooksaveoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/ebooksaveoptions/
---

## EbookSaveOptions class

Представляет параметры сохранения файла ebook.

```go

type EbookSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewEbookSaveOptions](./newebooksaveoptions/) | Создаёт параметры для сохранения ebook-файла. |
| [NewEbookSaveOptions_SaveFormat](./newebooksaveoptions_saveformat/) | Создаёт параметры для сохранения ebook-файла. |
| [NewEbookSaveOptions_HtmlSaveOptions](./newebooksaveoptions_htmlsaveoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Указывает, экспортировать ли невидимые фигуры |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Указывает, экспортировать ли невидимые фигуры |
| [GetPageTitle](./getpagetitle/) | Заголовок HTML-страницы. Только при сохранении в HTML-поток. |
| [SetPageTitle](./setpagetitle/) | Заголовок HTML-страницы. Только при сохранении в HTML-поток. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в HTML-поток. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в HTML-поток. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | Укажите префикс URL вложенных файлов, например изображений, в HTML-файле. Только при сохранении в HTML-поток. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | Укажите префикс URL вложенных файлов, например изображений, в HTML-файле. Только при сохранении в HTML-поток. |
| [GetDefaultFontName](./getdefaultfontname/) | Укажите имя шрифта по умолчанию для экспорта HTML; шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null. |
| [SetDefaultFontName](./setdefaultfontname/) | Укажите имя шрифта по умолчанию для экспорта HTML; шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null. |
| [GetAddGenericFont](./getaddgenericfont/) | Указывает, добавлять ли общий шрифт в CSS font-family. Значение по умолчанию — true. |
| [SetAddGenericFont](./setaddgenericfont/) | Указывает, добавлять ли общий шрифт в CSS font-family. Значение по умолчанию — true. |
| [GetWorksheetScalable](./getworksheetscalable/) | Указывает, увеличивается или уменьшается HTML с помощью уровня масштабирования листа при сохранении файла в HTML, значение по умолчанию — false. |
| [SetWorksheetScalable](./setworksheetscalable/) | Указывает, увеличивается или уменьшается HTML с помощью уровня масштабирования листа при сохранении файла в HTML, значение по умолчанию — false. |
| [IsExportComments](./isexportcomments/) | Указывает, экспортировать ли комментарии при сохранении файла в HTML, значение по умолчанию — false. |
| [SetIsExportComments](./setisexportcomments/) | Указывает, экспортировать ли комментарии при сохранении файла в HTML, значение по умолчанию — false. |
| [GetExportCommentsType](./getexportcommentstype/) | Представляет тип экспорта комментариев в HTML‑файлы. |
| [SetExportCommentsType](./setexportcommentstype/) | Представляет тип экспорта комментариев в HTML‑файлы. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Указывает, отключать ли раскрытые условные комментарии Downlevel при экспорте файла в HTML, значение по умолчанию — false. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Указывает, отключать ли раскрытые условные комментарии Downlevel при экспорте файла в HTML, значение по умолчанию — false. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | Указывает, экспортировать ли файлы изображений во временный каталог. Только при сохранении в поток HTML. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Указывает, экспортировать ли файлы изображений во временный каталог. Только при сохранении в поток HTML. |
| [GetImageScalable](./getimagescalable/) | Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true. |
| [SetImageScalable](./setimagescalable/) | Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true. |
| [GetWidthScalable](./getwidthscalable/) | Указывает, экспортировать ли ширину столбца в единицах масштаба в HTML. Значение по умолчанию — false. |
| [SetWidthScalable](./setwidthscalable/) | Указывает, экспортировать ли ширину столбца в единицах масштаба в HTML. Значение по умолчанию — false. |
| [GetExportSingleTab](./getexportsingletab/) | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false. |
| [SetExportSingleTab](./setexportsingletab/) | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Указывает, экспортировать ли только активный лист в HTML‑файл. Если true, то будет экспортирован только активный лист; если false, то будет экспортирована вся книга. Значение по умолчанию — false. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Указывает, экспортировать ли только активный лист в HTML‑файл. Если true, то будет экспортирован только активный лист; если false, то будет экспортирована вся книга. Значение по умолчанию — false. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | Указывает, экспортировать ли только область печати в HTML‑файл. Значение по умолчанию — false. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | Указывает, экспортировать ли только область печати в HTML‑файл. Значение по умолчанию — false. |
| [GetExportArea](./getexportarea/) | Получает или задает область CellArea для экспорта текущего активного листа. Если установить этот атрибут, область печати текущего активного листа будет опущена. При сохранении файла в HTML будет экспортирована только указанная область. |
| [SetExportArea](./setexportarea/) | Получает или задает область CellArea для экспорта текущего активного листа. Если установить этот атрибут, область печати текущего активного листа будет опущена. При сохранении файла в HTML будет экспортирована только указанная область. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | Указывает, следует ли парсить HTML‑теги (например <c>&lt;div&gt;&lt;/div&gt;</c>) в ячейке как значение ячейки или сохранять их как есть. Значение по умолчанию — true. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | Указывает, следует ли парсить HTML‑теги (например <c>&lt;div&gt;&lt;/div&gt;</c>) в ячейке как значение ячейки или сохранять их как есть. Значение по умолчанию — true. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате HTML. По умолчанию значение — Default, поэтому для строк, охватывающих несколько ячеек, разница между HTML‑файлами, созданными Aspose.Cells и MS Excel, небольшая. Однако при создании больших HTML‑файлов установка значения в Cross ускорит процесс в несколько раз по сравнению с Default или Fit2Cell. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате HTML. По умолчанию значение — Default, поэтому для строк, охватывающих несколько ячеек, разница между HTML‑файлами, созданными Aspose.Cells и MS Excel, небольшая. Однако при создании больших HTML‑файлов установка значения в Cross ускорит процесс в несколько раз по сравнению с Default или Fit2Cell. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Скрытый столбец (ширина этого столбца равна 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenColDisplayType имеет значение "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт. Значение по умолчанию — "Hidden". |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Скрытый столбец (ширина этого столбца равна 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenColDisplayType имеет значение "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт. Значение по умолчанию — "Hidden". |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Скрытая строка (высота этой строки равна 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта. Значение по умолчанию — "Hidden". |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Скрытая строка (высота этой строки равна 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта. Значение по умолчанию — "Hidden". |
| [GetEncoding](./getencoding/) | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [SetEncoding](./setencoding/) | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [GetImageOptions](./getimageoptions/) | Получите объект ImageOrPrintOptions перед экспортом. |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | Указывает, сохранять ли HTML как один файл. Значение по умолчанию — false. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | Указывает, сохранять ли HTML как один файл. Значение по умолчанию — false. |
| [GetShowAllSheets](./getshowallsheets/) | Указывает, отображать ли все листы при сохранении в один HTML‑файл. |
| [SetShowAllSheets](./setshowallsheets/) | Указывает, отображать ли все листы при сохранении в один HTML‑файл. |
| [GetExportPageHeaders](./getexportpageheaders/) | Указывает, экспортировать ли заголовки страниц. |
| [SetExportPageHeaders](./setexportpageheaders/) | Указывает, экспортировать ли заголовки страниц. |
| [GetExportPageFooters](./getexportpagefooters/) | Указывает, экспортировать ли заголовки страниц. |
| [SetExportPageFooters](./setexportpagefooters/) | Указывает, экспортировать ли заголовки страниц. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Указывает, экспортировать ли содержимое скрытого листа. Значение по умолчанию — true. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Указывает, экспортировать ли содержимое скрытого листа. Значение по умолчанию — true. |
| [GetPresentationPreference](./getpresentationpreference/) | Указывает, предпочтителен ли формат HTML или MHT для представления. Значение по умолчанию — false. Если вы хотите более красивое представление, установите значение в true. |
| [SetPresentationPreference](./setpresentationpreference/) | Указывает, предпочтителен ли формат HTML или MHT для представления. Значение по умолчанию — false. Если вы хотите более красивое представление, установите значение в true. |
| [GetCellCssPrefix](./getcellcssprefix/) | Получает и задает префикс имени CSS, значение по умолчанию — "". |
| [SetCellCssPrefix](./setcellcssprefix/) | Получает и задает префикс имени CSS, значение по умолчанию — "". |
| [GetTableCssId](./gettablecssid/) | Получает и задает префикс типа имени CSS, например tr, col, td и т.д., которые находятся в элементе table, имеющем атрибут TableCssId. Значение по умолчанию — "". |
| [SetTableCssId](./settablecssid/) | Получает и задает префикс типа имени CSS, например tr, col, td и т.д., которые находятся в элементе table, имеющем атрибут TableCssId. Значение по умолчанию — "". |
| [IsFullPathLink](./isfullpathlink/) | Указывает, использовать ли полные ссылки в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false. |
| [SetIsFullPathLink](./setisfullpathlink/) | Указывает, использовать ли полные ссылки в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. Значение по умолчанию — false. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. Значение по умолчанию — false. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в HTML. Значение по умолчанию — false. Если вы хотите импортировать полученный HTML в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в HTML. Значение по умолчанию — false. Если вы хотите импортировать полученный HTML в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExportExtraHeadings](./getexportextraheadings/) | Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать HTML‑файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportExtraHeadings](./setexportextraheadings/) | Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать HTML‑файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [GetExportFormula](./getexportformula/) | Указывает, экспортировать ли формулы при сохранении файла в HTML. Значение по умолчанию — true. Если вы хотите импортировать полученный HTML в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportFormula](./setexportformula/) | Указывает, экспортировать ли формулы при сохранении файла в HTML. Значение по умолчанию — true. Если вы хотите импортировать полученный HTML в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetAddTooltipText](./getaddtooltiptext/) | Указывает, добавлять ли подсказки, когда данные не могут быть полностью отображены. Значение по умолчанию — false. |
| [SetAddTooltipText](./setaddtooltiptext/) | Указывает, добавлять ли подсказки, когда данные не могут быть полностью отображены. Значение по умолчанию — false. |
| [GetExportGridLines](./getexportgridlines/) | Указывает, экспортировать ли линии сетки. Значение по умолчанию — false. |
| [SetExportGridLines](./setexportgridlines/) | Указывает, экспортировать ли линии сетки. Значение по умолчанию — false. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Указывает, исключать ли неиспользуемые стили. Для генерируемых HTML‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальные эффекты. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого HTML (например, в сценарии, когда пользователь позже восстанавливает рабочую книгу из сгенерированного HTML), установите это свойство в false. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Указывает, исключать ли неиспользуемые стили. Для генерируемых HTML‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальные эффекты. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого HTML (например, в сценарии, когда пользователь позже восстанавливает рабочую книгу из сгенерированного HTML), установите это свойство в false. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Указывает, экспортировать ли скрипты фрейма и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Указывает, экспортировать ли скрипты фрейма и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [GetExportDataOptions](./getexportdataoptions/) | Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All. |
| [SetExportDataOptions](./setexportdataoptions/) | Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All. |
| [GetLinkTargetType](./getlinktargettype/) | Указывает тип атрибута target в ссылке <c>&lt;a&gt;</c>. Значение по умолчанию — HtmlLinkTargetType.Parent. |
| [SetLinkTargetType](./setlinktargettype/) | Указывает тип атрибута target в ссылке <c>&lt;a&gt;</c>. Значение по умолчанию — HtmlLinkTargetType.Parent. |
| [IsIECompatible](./isiecompatible/) | Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false. |
| [SetIsIECompatible](./setisiecompatible/) | Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false. |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false. |
| [GetCalculateFormula](./getcalculateformula/) | Указывает, вычислять ли формулы перед сохранением HTML‑файла. |
| [SetCalculateFormula](./setcalculateformula/) | Указывает, вычислять ли формулы перед сохранением HTML‑файла. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true. |
| [IsMobileCompatible](./ismobilecompatible/) | Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false. |
| [SetIsMobileCompatible](./setismobilecompatible/) | Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false. |
| [GetCssStyles](./getcssstyles/) | Получает или задает дополнительные CSS‑стили для форматировщика. Работает только когда SaveAsSingleFile равно True. |
| [SetCssStyles](./setcssstyles/) | Получает или задает дополнительные CSS‑стили для форматировщика. Работает только когда SaveAsSingleFile равно True. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false. |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false. |
| [IsBorderCollapsed](./isbordercollapsed/) | Указывает, свернуты ли границы таблицы. Значение по умолчанию — true. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | Указывает, свернуты ли границы таблицы. Значение по умолчанию — true. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | Указывает, заменяются ли HTML‑символьные сущности на десятичный код (например, "&amp;nbsp;" заменяется на "&amp;#160;"). Значение по умолчанию — false. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | Указывает, заменяются ли HTML‑символьные сущности на десятичный код (например, "&amp;nbsp;" заменяется на "&amp;#160;"). Значение по умолчанию — false. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image. |
| [GetCellNameAttribute](./getcellnameattribute/) | Указывает атрибут, в котором записывается CellName (например, если значение "id", то для ячейки "A1" вывод будет: &lt;td id='A1'&gt;). Значение по умолчанию — null. |
| [SetCellNameAttribute](./setcellnameattribute/) | Указывает атрибут, в котором записывается CellName (например, если значение "id", то для ячейки "A1" вывод будет: &lt;td id='A1'&gt;). Значение по умолчанию — null. |
| [GetDisableCss](./getdisablecss/) | Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false. |
| [SetDisableCss](./setdisablecss/) | Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | Оптимизирует вывод HTML с помощью пользовательских CSS‑свойств. Например, если один base64‑изображение используется несколько раз, с пользовательским свойством данные изображения сохраняются один раз, что улучшает производительность получаемого HTML. Значение по умолчанию — false. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | Оптимизирует вывод HTML с помощью пользовательских CSS‑свойств. Например, если один base64‑изображение используется несколько раз, с пользовательским свойством данные изображения сохраняются один раз, что улучшает производительность получаемого HTML. Значение по умолчанию — false. |
| [GetHtmlVersion](./gethtmlversion/) | Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default. |
| [SetHtmlVersion](./sethtmlversion/) | Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default. |
| [GetSheetSet](./getsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | Получает или задает режим компоновки при сохранении в HTML. Значение по умолчанию — HtmlLayoutMode.Normal. |
| [SetLayoutMode](./setlayoutmode/) | Получает или задает режим компоновки при сохранении в HTML. Значение по умолчанию — HtmlLayoutMode.Normal. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Получает или задает тип встраивания файлов шрифтов в HTML‑файл. Значение по умолчанию — HtmlEmbeddedFontType.None, что означает, что шрифты в HTML не будут встраиваться. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Получает или задает тип встраивания файлов шрифтов в HTML‑файл. Значение по умолчанию — HtmlEmbeddedFontType.None, что означает, что шрифты в HTML не будут встраиваться. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении в HTML. Значение по умолчанию — true. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении в HTML. Значение по умолчанию — true. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | Представляет режим отображения DataBar при конвертации файлов Excel в HTML. Значение по умолчанию — DataBarRenderMode.BackgroundColor. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | Представляет режим отображения DataBar при конвертации файлов Excel в HTML. Значение по умолчанию — DataBarRenderMode.BackgroundColor. |
| [GetSpaceMode](./getspacemode/) | Указывает, как отображаются пробелы в выводе HTML. В данный момент эта опция применяется только к числовым форматам (например, бухгалтерский формат). Значение по умолчанию — HtmlSpaceMode.Css. |
| [SetSpaceMode](./setspacemode/) | Указывает, как отображаются пробелы в выводе HTML. В данный момент эта опция применяется только к числовым форматам (например, бухгалтерский формат). Значение по умолчанию — HtmlSpaceMode.Css. |
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
