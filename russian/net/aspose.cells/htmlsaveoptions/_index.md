---
title: "Класс HtmlSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HtmlSaveOptions. Представляет параметры для сохранения HTML‑файла"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Представляет параметры сохранения HTML‑файла.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Создаёт параметры для сохранения HTML‑файла. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Создаёт параметры для сохранения HTM‑файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Указывает, следует ли добавить общий шрифт в CSS‑font-family. Значение по умолчанию: true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Указывает, добавлять ли подсказку, когда данные не могут быть полностью отображены. Значение по умолчанию: false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток HTML. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Укажите префикс URL вложенных файлов, например изображений, в HTML‑файле. Только при сохранении в поток HTML. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Указывает, следует ли вычислять формулы перед сохранением HTML‑файла. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Получает и задаёт префикс имени CSS, значение по умолчанию — \"\". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Указывает атрибут, в котором будет записано имя ячейки (CellName). (например, если значение \"id\", то для ячейки \"A1\" вывод будет: &lt;td id='A1'&gt;). Значение по умолчанию — null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Получает или задаёт дополнительные CSS‑стили для форматировщика. Работает только когда [`SaveAsSingleFile`](./saveassinglefile/) равно True. CssStyles=\"body { padding: 5px }\"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Представляет режим отображения DataBar при конвертации файлов Excel в HTML‑файлы. Значение по умолчанию — BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Укажите имя шрифта по умолчанию для экспорта HTML; этот шрифт будет использоваться, если шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells использует универсальный шрифт той же семейства, что и оригинальный шрифт. Значение по умолчанию — null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Указывает, отключать ли условные комментарии Downlevel-revealed при экспорте файла в HTML, значение по умолчанию — false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Получает или задаёт тип встраивания файлов шрифтов в HTML‑файл. Значение по умолчанию — None, что означает, что шрифты не будут встраиваться в HTML. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Оптимизировать вывод HTML с помощью пользовательских свойств CSS. Например, если один base64‑изображение используется несколько раз, с пользовательским свойством данные изображения сохраняются один раз, что повышает производительность получаемого HTML. Значение по умолчанию — false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Указывает, заменяются ли HTML‑символьные сущности на десятичные коды. (например, \"&amp;nbsp;\" заменяется на \"&amp;#160;\"). Значение по умолчанию — false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Указывает, исключать ли неиспользуемые стили. Для генерируемых HTML‑файлов исключение неиспользуемых стилей уменьшает размер файла без влияния на визуальное отображение. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого HTML (например, чтобы позже восстановить книгу из HTML), установите значение свойства в false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Указывает, экспортировать ли только активный лист в HTML‑файл. Если true, будет экспортирован только активный лист; если false — будет экспортирована вся рабочая книга. Значение по умолчанию — false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Получает или задаёт область ячеек (CellArea) для экспорта текущего активного листа. Если задать этот атрибут, область печати текущего активного листа будет игнорироваться. При сохранении в HTML будет экспортирована только указанная область. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Представляет тип экспорта комментариев в html‑файлы. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Указывает правило экспорта данных html‑файла.Значение по умолчанию — All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Указывает, экспортировать ли свойства документа.Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Указывает, экспортировать ли формулы при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Указывает, экспортировать ли скрипты фрейма и свойства документа. Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Указывает, экспортировать ли линии сетки.Значение по умолчанию — false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Указывает, экспортировать ли скрытое содержимое листа.Значение по умолчанию — true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении как HTML. Значение по умолчанию — true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Получает или задает ExportObjectListener для экспорта объектов. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Указывает, экспортировать ли заголовки страниц. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Указывает, экспортировать ли заголовки страниц. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. Значение по умолчанию — false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Указывает, экспортировать ли свойства рабочей книги.Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Указывает, экспортировать ли CSS листа отдельно.Значение по умолчанию — false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Указывает, экспортировать ли свойства листа.Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Получает или задает IFilePathProvider для отдельного экспорта листа в html. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в html‑формат, если HtmlHiddenColDisplayType равно "Remove", скрытый столбец не будет выводиться, если значение "Hidden", столбец будет выводиться, но будет скрыт, значение по умолчанию — "Hidden". |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Скрытая строка (высота этой строки 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться, если значение "Hidden", строка будет выводиться, но будет скрыта, значение по умолчанию — "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Указывает, следует ли скрывать переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате HTML. По умолчанию значение — Default, поэтому для таких строк разница между HTML‑файлами, созданными Aspose.Cells и MS Excel, небольшая. Однако при создании больших HTML‑файлов установка значения Cross повышает производительность в несколько раз по сравнению с Default или Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Указывает, экспортировать ли невидимые фигуры |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Получите объект ImageOrPrintOptions перед экспортом |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Указывает, схлопнуты ли границы таблицы. Значение по умолчанию — true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Указывает, экспортировать ли файлы изображений во временный каталог. Только при сохранении в поток HTML. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Указывает, экспортировать ли комментарии при сохранении файла в HTML, значение по умолчанию — false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Указывает, использовать ли полные пути в ссылках в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false. |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Получает или задает режим компоновки при сохранении в HTML. Значение по умолчанию — Normal. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Указывает тип атрибута target в ссылке `<a>`. Значение по умолчанию — HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Указывает, следует ли принудительно объединять пустые элементы TD при экспорте файла в HTML. Размер HTML‑файла будет значительно уменьшен при установке значения true. Значение по умолчанию — false. Если вы хотите импортировать HTML‑файл в Excel или экспортировать идеальные линии сетки при сохранении в HTML, оставьте значение по умолчанию. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Указывает, как объекты OfficeMath экспортируются в HTML, значение по умолчанию — Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Заголовок HTML‑страницы. Только при сохранении в поток HTML. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Указывает, следует ли разбирать HTML‑теги (например, `<div></div>`) в ячейке как значение ячейки или сохранять их как есть. Значение по умолчанию — true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Указывает, предпочтителен ли формат html или mht для презентации. Значение по умолчанию — false. Если вы хотите получить более красивую презентацию, установите значение true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Указывает, сохранять ли HTML как один файл. Значение по умолчанию — false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Указывает, показывать ли все листы при сохранении в один HTML‑файл. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Указывает, как пробелы отображаются в выводе HTML. Эта опция в настоящее время применяется только к числовым форматам (например, бухгалтерский формат). Значение по умолчанию — Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Получает или задает IStreamProvider для экспорта объектов. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Получает и задает префикс имени типа css, например tr, col, td и т.д., они находятся в элементе table, который имеет атрибут TableCssId. Значение по умолчанию — "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Указывает, экспортировать ли ширину столбца в единицах масштаба в HTML. Значение по умолчанию — false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Указывает, следует ли масштабировать HTML с помощью уровня масштабирования листа при сохранении файла в HTML, значение по умолчанию — false. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Создайте экземпляр HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Сохраните книгу в формате HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


