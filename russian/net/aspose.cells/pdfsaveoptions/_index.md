---
title: "Класс PdfSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.PdfSaveOptions. Представляет параметры сохранения PDF‑файла"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Представляет параметры сохранения PDF‑файла.

```csharp
public class PdfSaveOptions : PaginatedSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Создаёт параметры для сохранения PDF‑файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Если значение AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в настройках pagesetup будет игнорироваться, а остальные настройки pagesetup по‑прежнему будут применяться. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark/) { get; set; } | Получает и задаёт объект [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry/). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula/) { get; set; } | Указывает, следует ли вычислять формулы перед сохранением PDF‑файла. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf, изображении. Установите значение true, чтобы попытаться сначала использовать шрифт по умолчанию книги для отображения этих символов. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance/) { get; set; } | Получает или задаёт уровень соответствия стандартам PDF для выходных документов. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime/) { get; set; } | Получает или задаёт время создания PDF‑документа. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport/) { get; set; } | Получает или задаёт значение, определяющее способ экспорта [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) в PDF‑файл. Значение по умолчанию — None. |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Получает или задаёт пользовательские настройки во время рендеринга. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Получает или задаёт язык редактирования по умолчанию. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle/) { get; set; } | Указывает, должно ли заголовок окна отображать название документа. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedAttachments](../../aspose.cells/pdfsaveoptions/embedattachments/) { get; set; } | Указывает, следует ли встраивать вложения для объектов Ole в Excel. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True — встраивать шрифты TrueType. Применяется только к символам ASCII 32‑127. Шрифты для кодов символов больше 127 всегда встраиваются. Шрифты всегда встраиваются для стандарта PDF/A-1a, PDF/A-1b. Значение по умолчанию — true. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Настройка рендеринга метафайла Emf. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure/) { get; set; } | Указывает, следует ли экспортировать структуру документа. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding/) { get; set; } | Получает или задаёт кодировку встроенных шрифтов в PDF. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Получает или задаёт цвет линий сетки. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Получает или задает тип линий сетки.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Указывает, нужно ли скрывать ошибку при рендеринге. Ошибка может быть связана с фигурой, изображением, рендерингом диаграммы и т.д.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ImageType](../../aspose.cells/pdfsaveoptions/imagetype/) { get; set; } | (**Obsolete.**) Представляет тип изображения при конвертации диаграммы и фигуры. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Указывает, следует ли заменять шрифт символа только тогда, когда шрифт ячейки несовместим с ним.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Если OnePagePerSheet установлен в true, всё содержимое листа будет выводиться только на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки страницы сохранят действие.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype/) { get; set; } | Получает и задаёт тип оптимизации PDF. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Указывает, следует ли выводить пустую страницу, когда нечего печатать.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Получает или задает количество страниц для сохранения.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Получает или задает нулевой индекс первой страницы для сохранения.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Управляет/указывает прогресс процесса сохранения страниц.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression/) { get; set; } | Укажите алгоритм сжатия |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Указывает, какие страницы не будут печататься.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Producer](../../aspose.cells/pdfsaveoptions/producer/) { get; set; } | Получает и задаёт производителя сгенерированного PDF‑документа. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Получает или задает специфические для Excel поведения рендеринга, которые следует применить.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions/) { get; set; } | Установите эти параметры, когда в результате xls2pdf требуется безопасность. |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |
| [Watermark](../../aspose.cells/pdfsaveoptions/watermark/) { get; set; } | Получает или задаёт водяной знак для вывода. |
| [ZoomBehavior](../../aspose.cells/pdfsaveoptions/zoombehavior/) { get; set; } | Получает или задаёт начальный режим просмотра при открытии сгенерированного PDF‑документа. Значение по умолчанию — None. |
| [ZoomFactor](../../aspose.cells/pdfsaveoptions/zoomfactor/) { get; set; } | Получает или задаёт процент масштабирования, используемый, когда [`ZoomBehavior`](./zoombehavior/) установлен в ZoomFactor. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample/)(int, int) | Устанавливает желаемое PPI (pixels per inch) для ресемплинга изображений и качество JPEG. Все изображения будут преобразованы в JPEG с указанным параметром качества, и изображения, у которых PPI превышает указанное значение (pixels per inch), будут ресемплированы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;
    using System.Drawing;

    public class PdfSaveOptionsDemo
    {
        public static void PdfSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Save Options Example");

            // Создайте экземпляр PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Установите различные свойства
            pdfSaveOptions.EmbedStandardWindowsFonts = true;
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            pdfSaveOptions.CalculateFormula = true;
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
            pdfSaveOptions.CreatedTime = DateTime.Now;
            pdfSaveOptions.Producer = "Aspose.Cells";
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
            pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
            pdfSaveOptions.ExportDocumentStructure = true;
            pdfSaveOptions.DisplayDocTitle = true;
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.EmbedAttachments = true;
            pdfSaveOptions.DefaultFont = "Arial";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;
            pdfSaveOptions.CheckFontCompatibility = true;
            pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.IgnoreError = true;
            pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
            pdfSaveOptions.PageIndex = 0;
            pdfSaveOptions.PageCount = 1;
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            pdfSaveOptions.GridlineType = GridlineType.Dotted;
            pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            pdfSaveOptions.ClearData = true;
            pdfSaveOptions.CachedFileFolder = "C:\\Temp";
            pdfSaveOptions.ValidateMergedAreas = true;
            pdfSaveOptions.MergeAreas = true;
            pdfSaveOptions.SortNames = true;
            pdfSaveOptions.SortExternalNames = true;
            pdfSaveOptions.RefreshChartCache = true;

            // Установите параметры безопасности
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
            {
                OwnerPassword = "OwnerPassword",
                UserPassword = "UserPassword",
                PrintPermission = true,
                FullQualityPrintPermission = true
            };
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Установите водяной знак
            RenderingFont font = new RenderingFont("Calibri", 68)
            {
                Italic = true,
                Bold = true,
                Color = Color.Blue
            };
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Rotation = 30,
                Opacity = 0.6f,
                ScaleToPagePercent = 50
            };
            pdfSaveOptions.Watermark = watermark;

            // Сохраните рабочую книгу в виде PDF-файла
            workbook.Save("PdfSaveOptionsExample.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


