---
title: "Класс EbookSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Saving.EbookSaveOptions. Представляет параметры для сохранения ebook-файла."
type: docs
url: /ru/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

Представляет параметры сохранения файла ebook.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | Создает параметры для сохранения файла электронной книги. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | Создает параметры для сохранения файла электронной книги. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Указывает, следует ли добавлять общий шрифт в CSS font-family. Значение по умолчанию — true (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Указывает, добавлять ли подсказку, когда данные не могут быть полностью отображены. Значение по умолчанию — false (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток html (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Укажите префикс Url для вложенных файлов, таких как изображения, в html‑файле. Только при сохранении в поток html (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Указывает, следует ли вычислять формулы перед сохранением html‑файла (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Получает и задает префикс имени css, значение по умолчанию — "" (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Указывает атрибут, который будет использоваться для записи имени ячейки. (например, если значение "id", то для ячейки "A1" вывод будет: &lt;td id='A1'&gt;). Значение по умолчанию — null (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Получает или задает дополнительные css‑стили для форматировщика. Работает только когда [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) установлен в True. CssStyles="body { padding: 5px }" (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Представляет режим отображения DataBar при конвертации файлов Excel в html. Значение по умолчанию — BackgroundColor (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Укажите имя шрифта по умолчанию для экспорта html, шрифт по умолчанию будет использован, если шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells использует универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Указывает, отключать ли раскрытые условные комментарии Downlevel при экспорте файла в html, значение по умолчанию — false (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Получает или задает тип встраивания файлов шрифтов в html‑файл. Значение по умолчанию — None, что означает, что шрифты не будут встраиваться в html (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Оптимизировать вывод html с помощью пользовательских свойств CSS. Например, в случае множественных вхождений одного изображения base64, с пользовательским свойством данные изображения сохраняются один раз, что улучшает производительность полученного html. Значение по умолчанию — false (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Указывает, заменяются ли HTML‑символьные сущности на десятичный код (например, "&amp;nbsp;" заменяется на "&amp;#160;"). Значение по умолчанию — false (наследуется от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Если не задано, используется Encoding.UTF8 в качестве типа кодировки по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Указывает, следует ли исключать неиспользуемые стили. Для генерируемых html‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальные эффекты. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого html (например, когда пользователь позже должен восстановить рабочую книгу из сгенерированного html), установите это свойство в false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Указывает, экспортировать ли только активный лист в html‑файл. Если true, будет экспортирован только активный лист; если false, будет экспортирована вся рабочая книга. Значение по умолчанию — false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Получает или задает область CellArea для экспорта текущего активного листа. Если задать этот атрибут, область печати текущего активного листа будет опущена. При сохранении файла в html будет экспортирована только указанная область.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Указывает, следует ли экспортировать фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Указывает, следует ли экспортировать координаты Excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать полученный html в Excel, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Представляет тип экспорта комментариев в html‑файлы.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Указывает правило экспорта данных html‑файла. Значение по умолчанию — All.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Указывает, следует ли экспортировать свойства документа. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Указывает, следует ли экспортировать дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Указывает, следует ли экспортировать формулы при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать полученный html в Excel, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Указывает, следует ли экспортировать скрипты фреймов и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Указывает, следует ли экспортировать линии сетки. Значение по умолчанию — false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Указывает, следует ли экспортировать заголовки строк и столбцов листа при сохранении в HTML‑файлы.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Указывает, следует ли экспортировать элементы‑якоря для именованных диапазонов при сохранении в HTML. Значение по умолчанию — true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Получает или задает ExportObjectListener для экспорта объектов.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Указывает, экспортировать ли заголовки страниц.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Указывает, экспортировать ли заголовки страниц.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Указывает, экспортировать ли только область печати в HTML‑файл. Значение по умолчанию — false.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать HTML или MHT файл в Excel, сохраните значение по умолчанию. Значение по умолчанию — false.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, сохраните значение по умолчанию.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, сохраните значение по умолчанию.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Получает или задает IFilePathProvider для отдельного экспорта листа в HTML.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в HTML‑формат, если HtmlHiddenColDisplayType установлен в "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт. Значение по умолчанию — "Hidden"(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Скрытая строка (высота этой строки 0) в Excel, перед сохранением в HTML‑формат, если HtmlHiddenRowDisplayType установлен в "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта. Значение по умолчанию — "Hidden"(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении Excel‑файла в HTML‑формате. По умолчанию значение — Default, поэтому для строк, охватывающих несколько ячеек, разница между HTML‑файлами, созданными Aspose.Cells и MS Excel, минимальна. Однако при создании больших HTML‑файлов установка значения в Cross дает производительность в несколько раз выше, чем при значении Default или Fit2Cell.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Указывает версию стандарта HTML, которую следует использовать при сохранении в HTML‑формате. Значение по умолчанию — HtmlVersion.Default.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Указывает, экспортировать ли невидимые фигуры.(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Получите объект ImageOrPrintOptions перед экспортом(Наследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Указывает, используется ли масштабируемая единица для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Указывает, свернуты ли границы таблицы. Значение по умолчанию — true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Указывает, экспортируются ли файлы изображений во временный каталог. Только при сохранении в поток html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Указывает, экспортировать ли комментарии при сохранении файла в html, значение по умолчанию — false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Получает или задает режим компоновки при сохранении в HTML. Значение по умолчанию — Normal (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Указывает тип атрибута target в ссылке `<a>`. Значение по умолчанию — HtmlLinkTargetType.Parent.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Указывает, выполнять ли принудительное объединение пустых элементов TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения true. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, пожалуйста, оставьте значение по умолчанию.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Заголовок html‑страницы. Только при сохранении в поток html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Указывает, следует ли разбирать html‑теги (например, `<div></div>`) в ячейке как значение ячейки или сохранять их как есть. Значение по умолчанию — true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Указывает, предпочтителен ли файл html или mht для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, пожалуйста, установите значение true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Указывает, сохранять ли html как один файл. Значение по умолчанию — false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Указывает, показывать ли все листы при сохранении в один html‑файл.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, следует ли сортировать определённые имена перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Указывает, как пробелы отображаются в HTML‑выводе. Эта опция в настоящее время применяется только к числовым форматам (например, бухгалтерский формат). Значение по умолчанию — Css.(Унаследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Получает или задаёт IStreamProvider для экспорта объектов.(Унаследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Получает и задаёт префикс имени типа css, например tr,col,td и т.д., они находятся в элементе table, который имеет атрибут TableCssId. Значение по умолчанию — "".(Унаследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, следует ли обновлять настройки SmartArt. Значение по умолчанию — false.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, следует ли проверять объединённые ячейки перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Указывает, следует ли экспортировать ширину столбца в единицах масштаба в HTML. Значение по умолчанию — false.(Унаследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Указывает, будет ли масштабировать HTML в соответствии с уровнем масштабирования листа при сохранении файла в HTML, значение по умолчанию — false.(Унаследовано от [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // Создайте экземпляр EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Установка свойств
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Сохраните книгу в HTML‑файл с указанными параметрами
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


