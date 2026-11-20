---
title: "EbookSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры сохранения файла электронного книги."
type: docs
url: /ru/java/com.aspose.cells/ebooksaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
```
public class EbookSaveOptions extends HtmlSaveOptions
```

Представляет параметры сохранения файла электронного книги.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EbookSaveOptions()](#EbookSaveOptions--) | Создаёт параметры для сохранения файла электронной книги. |
| [EbookSaveOptions(int saveFormat)](#EbookSaveOptions-int-) | Создаёт параметры для сохранения файла электронной книги. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Указывает, следует ли добавить общий шрифт в CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | Указывает, добавлять ли подсказку, когда данные не могут быть полностью отображены. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Каталог, в который будут сохраняться вложенные файлы. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Укажите префикс Url прикреплённых файлов, таких как изображения, в HTML‑файле. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [getCalculateFormula()](#getCalculateFormula--) | Указывает, следует ли вычислять формулы перед сохранением HTML‑файла. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Получает префикс имени css, значение по умолчанию — "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Указывает атрибут, определяющий CellName для записи. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getCssStyles()](#getCssStyles--) | Получает дополнительные стили css для форматировщика. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Представляет режим рендеринга DataBar при конвертации файлов Excel в HTML‑файлы. |
| [getDefaultFontName()](#getDefaultFontName--) | Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null. |
| [getDisableCss()](#getDisableCss--) | Указывает, применяются ли только встроенные стили без использования CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Указывает, отключать ли Downlevel-revealed условные комментарии при экспорте файла в HTML, значение по умолчанию — false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Получает тип встраивания файлов шрифтов в HTML‑файл. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Оптимизирует вывод HTML с помощью пользовательских свойств CSS. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Указывает, заменяются ли HTML‑символьные сущности на десятичные коды. |
| [getEncoding()](#getEncoding--) | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Указывает, исключать ли неиспользуемые стили. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Указывает, экспортировать ли только активный лист в HTML‑файл. |
| [getExportArea()](#getExportArea--) | Получает экспортируемую CellArea текущего активного Worksheet. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Указывает, экспортировать ли фиктивные данные нижней строки. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в HTML. |
| [getExportCommentsType()](#getExportCommentsType--) | Представляет тип экспорта комментариев в HTML‑файлы. |
| [getExportDataOptions()](#getExportDataOptions--) | Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. |
| [getExportFormula()](#getExportFormula--) | Указывает, экспортировать ли формулы при сохранении файла в HTML. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Указывает, экспортировать ли скрипты кадров и свойства документа. |
| [getExportGridLines()](#getExportGridLines--) | Указывает, экспортировать ли сетку. Значение по умолчанию — false. |
| [getExportHeadings()](#getExportHeadings--) | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении в HTML. |
| [getExportObjectListener()](#getExportObjectListener--) | Получает ExportObjectListener для экспорта объектов. |
| [getExportPageFooters()](#getExportPageFooters--) | Указывает, экспортировать ли заголовки страниц. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Указывает, экспортировать ли заголовки страниц. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Указывает, экспортировать ли только область печати в HTML‑файл. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Указывает, экспортировать ли аналогичный стиль границы, когда стиль границы не поддерживается браузерами. |
| [getExportSingleTab()](#getExportSingleTab--) | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [getFilePathProvider()](#getFilePathProvider--) | Получает IFilePathProvider для отдельного экспорта листа в HTML. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenColDisplayType имеет значение "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт; значение по умолчанию — "Hidden". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Скрытая строка (высота этой строки 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта; значение по умолчанию — "Hidden". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel, при сохранении файла Excel в формате HTML. |
| [getHtmlVersion()](#getHtmlVersion--) | Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Указывает, экспортировать ли невидимые фигуры. |
| [getImageOptions()](#getImageOptions--) | Получите объект ImageOrPrintOptions перед экспортом. |
| [getImageScalable()](#getImageScalable--) | Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. |
| [getLayoutMode()](#getLayoutMode--) | Получает режим макета при сохранении в HTML. |
| [getLinkTargetType()](#getLinkTargetType--) | Указывает тип целевого атрибута в ссылке `<a>`. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Указывает, следует ли принудительно объединять пустые элементы TD при экспорте файла в html. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image. |
| [getPageTitle()](#getPageTitle--) | Заголовок html‑страницы. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Указывает, следует ли парсить html‑тег (например, `<div></div>`) в ячейке как значение ячейки или сохранять его как есть. |
| [getPresentationPreference()](#getPresentationPreference--) | Указывает, предпочтителен ли файл html или mht для презентации. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, кэшировать ли последние данные диаграммы. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Указывает, сохранять ли html как один файл. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSheetSet()](#getSheetSet--) | Получает листы для рендеринга. |
| [getShowAllSheets()](#getShowAllSheets--) | Указывает, показывать ли все листы при сохранении в один html‑файл. |
| [getSortExternalNames()](#getSortExternalNames--) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getSpaceMode()](#getSpaceMode--) | Указывает, как пробелы отображаются в выводе HTML. |
| [getStreamProvider()](#getStreamProvider--) | Получает IStreamProvider для экспорта объектов. |
| [getTableCssId()](#getTableCssId--) | Получает префикс типа имени css, например tr, col, td и т.д., которые находятся в элементе table с атрибутом TableCssId. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Указывает, обновлять ли настройки SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [getWidthScalable()](#getWidthScalable--) | Указывает, экспортировать ли ширину столбцов в единицах масштаба в html. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Указывает, масштабировать ли html через уровень масштабирования листа при сохранении файла в html; значение по умолчанию — false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Указывает, схлопнуты ли границы таблицы. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Указывает, экспортировать ли файлы изображений во временный каталог. |
| [isExportComments()](#isExportComments--) | Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false. |
| [isFullPathLink()](#isFullPathLink--) | Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | Указывает, совместим ли выводимый HTML с браузером IE. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | Указывает, совместим ли выводимый HTML с мобильными устройствами. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Указывает, следует ли добавить общий шрифт в CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Указывает, добавлять ли подсказку, когда данные не могут быть полностью отображены. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Каталог, в который будут сохраняться вложенные файлы. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Укажите префикс Url прикреплённых файлов, таких как изображения, в HTML‑файле. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Указывает, схлопнуты ли границы таблицы. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Указывает, следует ли вычислять формулы перед сохранением HTML‑файла. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Устанавливает префикс имени css, значение по умолчанию — "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Указывает атрибут, определяющий CellName для записи. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Устанавливает дополнительные css‑стили для форматтера. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Представляет режим рендеринга DataBar при конвертации файлов Excel в HTML‑файлы. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Указывает, применяются ли только встроенные стили без использования CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Указывает, отключать ли Downlevel-revealed условные комментарии при экспорте файла в HTML, значение по умолчанию — false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Устанавливает тип встраивания файлов шрифтов в html‑файл. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Оптимизирует вывод HTML с помощью пользовательских свойств CSS. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Указывает, заменяются ли HTML‑символьные сущности на десятичные коды. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Указывает, исключать ли неиспользуемые стили. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Указывает, экспортировать ли файлы изображений во временный каталог. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Указывает, экспортировать ли только активный лист в HTML‑файл. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Устанавливает экспортируемую CellArea текущего активного Worksheet. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Указывает, экспортировать ли фиктивные данные нижней строки. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в HTML. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Представляет тип экспорта комментариев в HTML‑файлы. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Указывает, экспортировать ли формулы при сохранении файла в HTML. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Указывает, экспортировать ли скрипты кадров и свойства документа. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Указывает, экспортировать ли сетку. Значение по умолчанию — false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении в HTML. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Устанавливает ExportObjectListener для экспорта объектов. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Указывает, экспортировать ли заголовки страниц. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Указывает, экспортировать ли заголовки страниц. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Указывает, экспортировать ли только область печати в HTML‑файл. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Указывает, экспортировать ли аналогичный стиль границы, когда стиль границы не поддерживается браузерами. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Устанавливает IFilePathProvider для отдельного экспорта Worksheet в html. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenColDisplayType имеет значение "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт; значение по умолчанию — "Hidden". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Скрытая строка (высота этой строки 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта; значение по умолчанию — "Hidden". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel, при сохранении файла Excel в формате HTML. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Указывает, совместим ли выводимый HTML с браузером IE. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Указывает, экспортировать ли невидимые фигуры. |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | Устанавливает режим компоновки при сохранении в HTML. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Указывает тип целевого атрибута в ссылке `<a>`. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Указывает, следует ли принудительно объединять пустые элементы TD при экспорте файла в html. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Указывает, совместим ли выводимый HTML с мобильными устройствами. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Заголовок html‑страницы. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Указывает, следует ли парсить html‑тег (например, `<div></div>`) в ячейке как значение ячейки или сохранять его как есть. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Указывает, предпочтителен ли файл html или mht для презентации. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, кэшировать ли последние данные диаграммы. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Указывает, сохранять ли html как один файл. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Устанавливает листы для рендеринга. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Указывает, показывать ли все листы при сохранении в один html‑файл. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Указывает, как пробелы отображаются в выводе HTML. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Устанавливает IStreamProvider для экспорта объектов. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Устанавливает префикс типа имени CSS, например tr, col, td и т.д.; они находятся в элементе table, который имеет специфический атрибут TableCssId. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Указывает, обновлять ли настройки SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Указывает, экспортировать ли ширину столбцов в единицах масштаба в html. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Указывает, масштабировать ли html через уровень масштабирования листа при сохранении файла в html; значение по умолчанию — false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookSaveOptions() {#EbookSaveOptions--}
```
public EbookSaveOptions()
```


Создаёт параметры для сохранения файла электронной книги.

### EbookSaveOptions(int saveFormat) {#EbookSaveOptions-int-}
```
public EbookSaveOptions(int saveFormat)
```


Создаёт параметры для сохранения файла электронной книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Формат файла. Должен быть [SaveFormat.EPUB](../../com.aspose.cells/saveformat\#EPUB) или [SaveFormat.AZW\_3](../../com.aspose.cells/saveformat\#AZW-3). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


Указывает, следует ли добавить общий шрифт в CSS font-family. Значение по умолчанию — true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Указывает, добавлять ли текст подсказки, когда данные не могут быть полностью отображены. Значение по умолчанию — false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток html.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Укажите префикс Url вложенных файлов, например изображений в html‑файле. Только при сохранении в поток html.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Указывает, следует ли вычислять формулы перед сохранением HTML‑файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Получает префикс имени css, значение по умолчанию — "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Указывает атрибут, в котором будет записано имя ячейки (CellName). (например, если значение "id", то для ячейки "A1" вывод будет: <td id='A1'>). Значение по умолчанию — null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Очищать книгу после сохранения файла.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Получает дополнительные css стили для форматировщика. Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) возвращает True. CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Представляет режим рендеринга DataBar при конвертации файлов Excel в html. Значение по умолчанию — [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

См. [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Указывает, отключать ли Downlevel-revealed условные комментарии при экспорте файла в HTML, значение по умолчанию — false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Получает тип встраивания файлов шрифтов в html‑файл. Значение по умолчанию — [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE), что означает отсутствие встраиваемых шрифтов в html.

См. [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


Оптимизирует вывод html с помощью пользовательских свойств CSS. Например, если один base64‑изображение используется несколько раз, с пользовательским свойством данные изображения сохраняются один раз, что повышает производительность получаемого html. Значение по умолчанию — false.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


Указывает, заменяются ли HTML‑символьные сущности на десятичные коды. (например, "&nbsp;" заменяется на "&\#160;"). Значение по умолчанию — false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Указывает, исключать ли неиспользуемые стили. Для генерируемых html‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальное отображение. Поэтому значение свойства по умолчанию — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого html (например, когда требуется восстановить рабочую книгу из сгенерированного html позже), установите значение свойства в false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Указывает, экспортировать ли только активный лист в html‑файл. Если true, будет экспортирован только активный лист; если false, будет экспортирована вся рабочая книга. Значение по умолчанию — false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Получает экспортируемую CellArea текущего активного Worksheet. Если задать этот атрибут, область печати текущего активного Worksheet будет исключена. При сохранении файла в html будет экспортирована только указанная область.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Представляет тип экспорта комментариев в HTML‑файлы.

Смотрите [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All.

Смотрите [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Указывает, экспортировать ли формулы при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Указывает, экспортировать ли скрипты фрейма и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Указывает, экспортировать ли сетку. Значение по умолчанию — false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство HtmlSaveOptions.ExportRowColumnHeadings. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose извиняется за любые причинённые неудобства.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB.

**Remarks**

Когда это свойство установлено в true, данные изображения экспортируются непосредственно в элементы img, и отдельные файлы не создаются.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении в HTML. Значение по умолчанию — true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Получает ExportObjectListener для экспорта объектов.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство HtmlSaveOptions.IStreamProvider. Это свойство будет удалено через 12 месяцев, начиная с августа 2015 года. Aspose извиняется за любые причинённые неудобства.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Указывает, экспортировать ли заголовки страниц.

**Remarks**

Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) установлено в True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Указывает, экспортировать ли заголовки страниц.

**Remarks**

Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) установлено в True.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию. Значение по умолчанию — false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Получает IFilePathProvider для отдельного экспорта листа в HTML.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenColDisplayType имеет значение "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт; значение по умолчанию — "Hidden".

Смотрите [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Скрытая строка (высота этой строки 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта; значение по умолчанию — "Hidden".

Смотрите [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false.

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате html. По умолчанию значение — Default, поэтому для таких строк разница между html‑файлами, созданными Aspose.Cells и MS Excel, минимальна. Однако при создании больших html‑файлов установка значения в Cross повышает производительность в несколько раз по сравнению с Default или Fit2Cell.

Смотрите [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default.

Смотрите [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Указывает, экспортировать ли невидимые фигуры.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Получите объект ImageOrPrintOptions перед экспортом.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


Получает режим компоновки при сохранении в HTML. Значение по умолчанию — [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Смотрите [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


Указывает тип атрибута target в ссылке `<a>`. Значение по умолчанию — HtmlLinkTargetType.Parent.

Смотрите [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Указывает, следует ли принудительно объединять пустой элемент TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения в true. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, пожалуйста, оставьте значение по умолчанию.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default.

Смотрите [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image.

Смотрите [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Заголовок html‑страницы. Используется только при сохранении в поток html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Указывает, следует ли парсить html‑тег (например `<div></div>`) в ячейке как значение ячейки или сохранять его как есть. Значение по умолчанию — true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Указывает, является ли html или mht файл предпочтительным для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Указывает, кэшировать ли последние данные диаграммы.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


Указывает, сохранять ли html как один файл. Значение по умолчанию — false.

**Remarks**

Если в рабочей книге несколько листов или другие необходимые ресурсы, такие как изображения, обычно эти листы и ресурсы сохраняются в отдельные файлы. В некоторых сценариях пользователю может потребоваться получить только один результирующий файл, например для удобства передачи. В этом случае пользователь может установить это свойство в true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает формат сохраняемого файла.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Получает листы для рендеринга. По умолчанию — все видимые листы в рабочей книге: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Указывает, показывать ли все листы при сохранении в один html‑файл.

**Remarks**

Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) установлено в True.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Указывает, сортировать ли внешние определённые имена перед сохранением файла.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


Указывает, как пробелы отображаются в выводе HTML. В настоящее время эта опция применяется только к числовым форматам (например, бухгалтерский формат). Значение по умолчанию — [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Смотрите [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Получает IStreamProvider для экспорта объектов.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Получает префикс типа имени css, например tr, col, td и т.д., которые находятся в элементе table, имеющем специфический атрибут TableCssId. Значение по умолчанию — "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Указывает, следует ли обновлять настройки Smart Art. Значение по умолчанию — false.

**Remarks**

Влияет только после вызова метода Shape.GetResultOfSmartArt() и если кэшированные фигуры существуют в файле шаблона.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Получает обратный вызов предупреждения.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Указывает, экспортировать ли ширину столбца в единицах масштаба в html. Значение по умолчанию — false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Указывает, масштабировать ли html через уровень масштабирования листа при сохранении файла в html; значение по умолчанию — false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


Указывает, схлопываются ли границы таблицы. Значение по умолчанию — true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Указывает, экспортировать ли файлы изображений во временный каталог. Используется только при сохранении в поток html.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false.

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


Указывает, следует ли добавить общий шрифт в CSS font-family. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Указывает, добавлять ли текст подсказки, когда данные не могут быть полностью отображены. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Каталог, в который будут сохраняться вложенные файлы. Только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Укажите префикс Url вложенных файлов, например изображений в html‑файле. Только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Указывает, схлопываются ли границы таблицы. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Указывает, следует ли вычислять формулы перед сохранением HTML‑файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Устанавливает префикс имени css, значение по умолчанию — "".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Указывает атрибут, в котором будет записано имя ячейки (CellName). (например, если значение "id", то для ячейки "A1" вывод будет: <td id='A1'>). Значение по умолчанию — null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Очищать книгу после сохранения файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Устанавливает дополнительные css‑стили для форматтера. Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) возвращает True. CssStyles="body \{ padding: 5px \}";

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Представляет режим рендеринга DataBar при конвертации файлов Excel в html. Значение по умолчанию — [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

См. [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Укажите имя шрифта по умолчанию для экспорта HTML, шрифт по умолчанию будет использоваться, когда шрифт стиля отсутствует. Если это свойство равно null, Aspose.Cells будет использовать универсальный шрифт той же семейства, что и оригинальный шрифт; значение по умолчанию — null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Указывает, отключать ли Downlevel-revealed условные комментарии при экспорте файла в HTML, значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Устанавливает тип встраивания файлов шрифтов в html‑файл. Значение по умолчанию — [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE), что означает, что шрифты не будут встраиваться в html.

См. [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


Оптимизирует вывод html с помощью пользовательских свойств CSS. Например, если один base64‑изображение используется несколько раз, с пользовательским свойством данные изображения сохраняются один раз, что повышает производительность получаемого html. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


Указывает, заменяются ли HTML‑символьные сущности на десятичные коды. (например, "&nbsp;" заменяется на "&\#160;"). Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Если не задано, используется Encoding.UTF8 в качестве кодировки по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Указывает, исключать ли неиспользуемые стили. Для генерируемых html‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальное отображение. Поэтому значение свойства по умолчанию — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого html (например, когда требуется восстановить рабочую книгу из сгенерированного html позже), установите значение свойства в false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Указывает, экспортировать ли файлы изображений во временный каталог. Используется только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Указывает, экспортировать ли только активный лист в html‑файл. Если true, будет экспортирован только активный лист; если false, будет экспортирована вся рабочая книга. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Устанавливает экспортируемую CellArea текущего активного листа Worksheet. Если задать этот атрибут, область печати текущего активного листа будет опущена. При сохранении файла в html будет экспортирована только указанная область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Указывает, экспортировать ли комментарии при сохранении файла в html; значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Представляет тип экспорта комментариев в HTML‑файлы.

Смотрите [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All.

Смотрите [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Указывает, экспортировать ли формулы при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Указывает, экспортировать ли скрипты фрейма и свойства документа. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Указывает, экспортировать ли сетку. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство HtmlSaveOptions.ExportRowColumnHeadings. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose извиняется за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Указывает, экспортировать ли скрытое содержимое листа. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Указывает, сохранять ли изображения в формате Base64 в HTML, MHTML или EPUB.

**Remarks**

Когда это свойство установлено в true, данные изображения экспортируются непосредственно в элементы img, и отдельные файлы не создаются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


Указывает, экспортировать ли элементы‑якоря для именованных диапазонов при сохранении в HTML. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Устанавливает ExportObjectListener для экспорта объектов.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство HtmlSaveOptions.IStreamProvider. Это свойство будет удалено через 12 месяцев, начиная с августа 2015 года. Aspose извиняется за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Указывает, экспортировать ли заголовки страниц.

**Remarks**

Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) установлено в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Указывает, экспортировать ли заголовки страниц.

**Remarks**

Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) установлено в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать html или mht файл в Excel, пожалуйста, оставьте значение по умолчанию. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Указывает, экспортировать ли CSS листа отдельно. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Указывает, экспортировать ли свойства листа. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Устанавливает IFilePathProvider для отдельного экспорта Worksheet в html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Указывает, использовать ли полные пути ссылок в sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Скрытый столбец (ширина этого столбца 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenColDisplayType имеет значение "Remove", скрытый столбец не будет выводиться; если значение "Hidden", столбец будет выводиться, но будет скрыт; значение по умолчанию — "Hidden".

Смотрите [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Скрытая строка (высота этой строки 0) в Excel, перед сохранением в формат HTML, если HtmlHiddenRowDisplayType имеет значение "Remove", скрытая строка не будет выводиться; если значение "Hidden", строка будет выводиться, но будет скрыта; значение по умолчанию — "Hidden".

Смотрите [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Указывает, скрывать ли переполняющий текст, когда формат ячейки установлен на перенос текста. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате html. По умолчанию значение — Default, поэтому для таких строк разница между html‑файлами, созданными Aspose.Cells и MS Excel, минимальна. Однако при создании больших html‑файлов установка значения в Cross повышает производительность в несколько раз по сравнению с Default или Fit2Cell.

Смотрите [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


Указывает версию стандарта HTML, которая должна использоваться при сохранении в формате HTML. Значение по умолчанию — HtmlVersion.Default.

Смотрите [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Указывает, экспортировать ли невидимые фигуры.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


Указывает, совместим ли JavaScript с браузерами, не поддерживающими JavaScript. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


Устанавливает режим макета при сохранении в HTML. Значение по умолчанию — [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Смотрите [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Указывает тип атрибута target в ссылке `<a>`. Значение по умолчанию — HtmlLinkTargetType.Parent.

Смотрите [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Указывает, следует ли принудительно объединять пустой элемент TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения в true. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, пожалуйста, оставьте значение по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default.

Смотрите [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image.

Смотрите [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Заголовок html‑страницы. Используется только при сохранении в поток html.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Указывает, следует ли парсить html‑тег (например `<div></div>`) в ячейке как значение ячейки или сохранять его как есть. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Указывает, является ли html или mht файл предпочтительным для представления. Значение по умолчанию — false. Если вы хотите получить более красивое представление, установите значение в true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Указывает, кэшировать ли последние данные диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Указывает, сохранять ли html как один файл. Значение по умолчанию — false.

**Remarks**

Если в рабочей книге несколько листов или другие необходимые ресурсы, такие как изображения, обычно эти листы и ресурсы сохраняются в отдельные файлы. В некоторых сценариях пользователю может потребоваться получить только один результирующий файл, например для удобства передачи. В этом случае пользователь может установить это свойство в true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Устанавливает листы для отображения. По умолчанию — все видимые листы в рабочей книге: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Указывает, показывать ли все листы при сохранении в один html‑файл.

**Remarks**

Работает только когда [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) установлено в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Указывает, сортировать ли внешние определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


Указывает, как пробелы отображаются в выводе HTML. В настоящее время эта опция применяется только к числовым форматам (например, бухгалтерский формат). Значение по умолчанию — [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Смотрите [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Устанавливает IStreamProvider для экспорта объектов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Устанавливает префикс имени CSS‑типа, например tr, col, td и т.д., они находятся в элементе table, который имеет атрибут TableCssId. Значение по умолчанию — "".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Указывает, следует ли обновлять настройки Smart Art. Значение по умолчанию — false.

**Remarks**

Влияет только после вызова метода Shape.GetResultOfSmartArt() и если кэшированные фигуры существуют в файле шаблона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Устанавливает обратный вызов предупреждения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Указывает, экспортировать ли ширину столбца в единицах масштаба в html. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Указывает, масштабировать ли html через уровень масштабирования листа при сохранении файла в html; значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

