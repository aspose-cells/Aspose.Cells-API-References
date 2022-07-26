---
title: HtmlSaveOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры сохранения HTML-файла.
type: docs
weight: 3740
url: /ru/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Представляет параметры сохранения HTML-файла.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Создает параметры для сохранения html-файла. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | Создает параметры для сохранения htm-файла. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Указывает, следует ли добавлять текст всплывающей подсказки, когда данные не могут быть полностью отображены. Значение по умолчанию — false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | Каталог, в который будут сохраняться вложенные файлы. Только для сохранения в поток html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | Укажите префикс URL вложенных файлов, таких как изображение в файле html. Только для сохранения в поток html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Папка с кэшированными файлами используется для хранения больших данных. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | Получает и устанавливает префикс имени css, значение по умолчанию "". |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Сделайте рабочую книгу пустой после сохранения файла. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Укажите имя шрифта по умолчанию для экспорта html, шрифт по умолчанию будет использоваться, когда шрифт стиля не существует, Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт, который имеет то же семейство, что и исходный шрифт, значение по умолчанию равно null. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Указывает, что при отключении условных комментариев, отображаемых на нижнем уровне, при экспорте файла в html значение по умолчанию равно false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Если не задано, используйте Encoding.UTF8 в качестве типа кодирования по умолчанию. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Указывает, исключаются ли неиспользуемые стили. Для сгенерированных html-файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальные эффекты. Таким образом, значение этого свойства по умолчанию равно true. Если пользователю необходимо сохранить все стили в рабочей книге для сгенерированного HTML-кода (например, сценарий, в котором user необходимо позже восстановить рабочую книгу из сгенерированного HTML-кода), установите для этого свойства значение false. . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Указывает, экспортируется ли вся книга в файл html. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Получает или задает экспортируемую CellArea текущего активного рабочего листа. Если установить этот атрибут, область печати текущего активного рабочего листа будет опущена. Только указанная область будет экспортирована при сохранении файла в формате html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Указывает, экспортируются ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, оставьте значение по умолчанию. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Указывает, экспортируются ли координаты excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать выходной HTML-код в Excel, оставьте значение по умолчанию. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Указывает правило экспорта данных файла html. Значение по умолчанию — All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Указывает, экспортируются ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, сохраните значение по умолчанию. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Указывает, следует ли экспортировать дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать HTML-файл в Excel, оставьте значение по умолчанию. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Указывает, экспортируется ли формула при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать выходной HTML-код в Excel, оставьте значение по умолчанию. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Указывает, экспортируются ли сценарии фреймов и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, оставьте значение по умолчанию. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Указывает, экспортируются ли линии сетки. Значение по умолчанию — false. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Указывает, экспортируется ли скрытое содержимое рабочего листа. Значение по умолчанию — true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Указывает, экспортируются ли заголовки страниц. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Указывает, экспортируются ли заголовки страниц. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Указывает, экспортируется ли только область печати в html-файл. Значение по умолчанию — false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | Указывает, экспортируются ли заголовки строк и столбцов листа при сохранении в файлы HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Указывает, экспортируется ли аналогичный стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать файл html или mht в Excel, оставьте значение по умолчанию. Значение по умолчанию — false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Указывает, следует ли экспортировать одну вкладку, когда файл содержит только один рабочий лист. Значение по умолчанию — false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Указывает, экспортируются ли свойства книги. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, сохраните значение по умолчанию. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Указывает, следует ли экспортировать рабочий лист css отдельно. Значение по умолчанию — false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Указывает, экспортируются ли свойства рабочего листа. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, сохраните значение по умолчанию. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Получает или задает IFilePathProvider для отдельного экспорта рабочего листа в html. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Скрытый столбец (ширина этого столбца равна 0) в Excel, перед сохранением в формате html, , если для HtmlHiddenColDisplayType установлено значение «Удалить», скрытый столбец не будет выводиться, , если значение «Скрытый», столбец будет был выведен, но был скрыт, значение по умолчанию "Скрытый" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Скрытая строка (высота этой строки равна 0) в Excel, перед сохранением в формате html, , если HtmlHiddenRowDisplayType имеет значение «Удалить», скрытая строка не будет выводиться, , если значение «Скрыто», строка будет был выведен, но был скрыт, значение по умолчанию "Скрытый" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Указывает, будет ли межъячеечная строка отображаться так же, как в MS Excel, при сохранении файла Excel в формате html. файлы, созданные Aspose.Cells и MS Excel. Но производительность при создании больших html-файлов при установке значения Cross будет в несколько раз выше, чем при установке значения Default или Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Укажите, экспортируются ли невидимые фигуры |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Получить объект ImageOrPrintOptions перед экспортом |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Указывает, используются ли масштабируемые единицы для описания ширины изображения при использовании масштабируемых единиц для описания ширины столбца. Значение по умолчанию — true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Указывает, экспортируются ли файлы изображений во временный каталог. Только для сохранения в поток html. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Указывает, что при экспорте комментариев при сохранении файла в html значение по умолчанию равно false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Указывает, используется ли полный путь в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | Указывает тип целевого атрибута в ссылке &lt;a&gt;. Значение по умолчанию — HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Указывает, будет ли принудительно объединяться пустой элемент TD при экспорте файла в html. Размер html-файла будет значительно уменьшен после установки значения true. Значение по умолчанию неверно. Если вы хотите импортировать html-файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, оставьте значение по умолчанию. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | Заголовок html-страницы. Только для сохранения в html-поток. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | Разобрать HTML-тег в ячейке, например , как значение ячейки или как HTML-тег, по умолчанию true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | Указывает, является ли файл html или mht предпочтительным для презентации. Значение по умолчанию — false. Если вы хотите получить более красивую презентацию, установите значение true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Указывает, нужно ли обновлять кэш диаграммы data |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Указывает, следует ли сохранять html как один файл. Значение по умолчанию — false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Получает формат файла сохранения. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Указывает, будут ли отображаться все листы при сохранении в виде одного HTML-файла. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Указывает, выполняется ли сортировка внешних определенных имен перед сохранением файла. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Указывает, выполняется ли сортировка определенных имен перед сохранением файла. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Получает или задает IStreamProvider для экспорта объектов. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | Получает и устанавливает префикс имени типа css, такой как tr, col, td и т. д., они содержатся в элементе таблицы , который имеет определенный атрибут TableCssId. Значение по умолчанию: "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Указывает, обновляются ли настройки Smart Art. Значение по умолчанию — false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Указывает, следует ли проверять объединенные ячейки перед сохранением файла. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Указывает, используются ли масштабируемые единицы для описания ширины столбца при экспорте файла в html. Значение по умолчанию — false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Указывает, что при увеличении или уменьшении масштаба html с помощью уровня масштабирования рабочего листа при сохранении файла в html значение по умолчанию равно false. |

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
