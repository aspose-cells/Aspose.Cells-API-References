---
title: PdfSaveOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры сохранения файла PDF.
type: docs
weight: 4500
url: /ru/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Представляет параметры сохранения файла PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Создает параметры для сохранения файла PDF. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | Если AllColumnsInOnePagePerSheet имеет значение true , все содержимое столбцов одного листа будет выведено только на одну страницу в результате. Ширина размера бумаги pagesetup будет игнорироваться, а другие настройки pagesetup по-прежнему будут действовать. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Получает и задает объект[`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry) . |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Папка с кэшированными файлами используется для хранения больших данных. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Указывает, следует ли вычислять формулы перед сохранением файла PDF. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | Когда символы в Excel имеют формат Unicode и для них не установлен правильный шрифт в стиле ячейки, Они могут отображаться как блоки в pdf, изображении. Установите для этого параметра значение true, чтобы попытаться использовать шрифт рабочей книги по умолчанию для отображения этих символов в первую очередь. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Сделайте рабочую книгу пустой после сохранения файла. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | Рабочая книга преобразуется в pdf в соответствии с PdfCompliance в этом свойстве. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Получает и устанавливает время создания pdf-документа. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Получает или задает значение, определяющее способ экспорта[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection)в файл PDF. Значение по умолчанию — Нет. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Получает или устанавливает язык редактирования по умолчанию. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | Когда символы в Excel имеют формат Unicode и для них не установлен правильный шрифт в стиле ячейки, Они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, для отображения этих символов. Если это свойство не установлено, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих символов Юникода. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Указывает, должна ли строка заголовка окна отображать заголовок документа. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True для встраивания шрифтов истинного типа. Влияет только на символы ASCII 32-127. Шрифты для кодов символов больше 127 всегда встраиваются. Шрифты всегда встроены для стандарта PDF/A-1a, PDF/A-1b. Значение по умолчанию — true. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Настройка для рендеринга метафайла EMF. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Указывает, следует ли экспортировать структуру документа. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | Получает или задает кодировку встроенного шрифта в pdf. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Получает или задает тип линии сетки. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Указывает, нужно ли скрыть ошибку при рендеринге. Ошибка может быть ошибкой формы, изображения, рендеринга диаграммы и т. д. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Указывает, следует ли заменять шрифт символа только в том случае, если шрифт ячейки несовместим с ним. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | Если OnePagePerSheet имеет значение true , все содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет неверным, а другие настройки pagesetup по-прежнему будут действовать. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | Получает и устанавливает тип оптимизации pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Указывает, выводить ли пустую страницу, когда печатать нечего. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Получает или задает количество сохраняемых страниц. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Получает или задает отсчитываемый от 0 индекс первой страницы для сохранения. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Управление/указание хода процесса сохранения страницы. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Указать алгоритм сжатия |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Указывает, какие страницы не будут распечатаны. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Получает и устанавливает производителя сгенерированного pdf-документа. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Указывает, обновляются ли данные кэша диаграммы |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Получает формат файла сохранения. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | Установите эту опцию, когда требуется безопасность в результате xls2pdf. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Указывает, выполняется ли сортировка внешних определенных имен перед сохранением файла. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Указывает, выполняется ли сортировка определенных имен перед сохранением файла. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Получает или задает отображаемый тип текста, когда ширина текста больше ширины ячейки. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Указывает, обновляются ли настройки смарт-арта. Значение по умолчанию — false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Указывает, следует ли проверять объединенные ячейки перед сохранением файла. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Получает или устанавливает обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Устанавливает желаемое значение PPI (пикселей на дюйм) изображений с повторной выборкой и качество JPEG. Все изображения будут преобразованы в JPEG с указанной настройкой качества, и изображения, превышающие указанный PPI (пикселей на дюйм), будут подвергнуты передискретизации. |

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
