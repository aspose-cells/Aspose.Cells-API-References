---
title: "Класс SvgImageOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.SvgImageOptions. Параметры для генерации SVG‑изображения"
type: docs
url: /ru/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Параметры генерации изображения SVG.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина бумаги, указанная в настройках страницы, будет недействительной, а остальные настройки страницы по‑прежнему будут применяться. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Указывает тип изображения диаграммы при конвертации. значение по умолчанию: PNG. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF, изображении. Установите значение true, чтобы попытаться сначала использовать шрифт книги по умолчанию для отображения этих символов. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Получает и задает префикс имени CSS в SVG, значение по умолчанию — пустая строка. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Клиент может выполнять специальный вывод на принтер при печати каждой страницы, используя этот обработчик событий (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Клиент может управлять настройками страницы принтера при печати каждой страницы, используя этот обработчик событий (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Получает или задает пользовательские настройки во время рендеринга. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Получает или задает язык редактирования по умолчанию. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Получает или задает тип шрифта, встроенного в SVG. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Указывает имя файла встроенного изображения в SVG. Должен быть полный путь с каталогом, например "c:\\xpsEmbedded" (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Настройка рендеринга EMF‑метафайлов в исходном файле. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Получает или задает EmfType, указывающий формат метафайла. Значение по умолчанию — EmfPlusDual. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Если это свойство равно true, сгенерированный SVG будет подгоняться под область просмотра. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Получает или задает цвет линий сетки. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Получает или задает тип линий сетки. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Получает или задает горизонтальное разрешение сгенерированных изображений в точках на дюйм. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Получает или задает формат сгенерированных изображений. значение по умолчанию: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Указывает, автоматически ли подгоняется ширина и высота ячеек по значению ячейки. Значение по умолчанию — false. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Указывает, заменять ли шрифт символа только когда шрифт ячейки несовместим с ним. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Указывает, оптимизировать ли выходные элементы. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Если это свойство равно true, будет выведена одна область, и масштаб не будет применяться. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Указывает, следует ли выводить пустую страницу, когда нечего печатать. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Получает или задаёт количество страниц для сохранения. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Получает или задаёт нулевой индекс первой страницы для сохранения. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Управляет/отображает прогресс процесса сохранения страниц. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Получает или задаёт формат пикселей для создаваемых изображений. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Указывает, какие страницы не будут печататься. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Если PrintWithStatusDialog = true, будет отображён диалог, показывающий текущий статус печати. иначе такой диалог не будет показываться. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Получает или задаёт значение, определяющее качество создаваемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. Значение по умолчанию — 100. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Получает или задаёт тип формата выходного файла. Поддерживает Tiff/XPS. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в рабочей книге: [`Visible`](../sheetset/visible/). (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Указывает, применяется ли сглаживание (антиалиасинг) к линиям, кривым и краям заполненных областей. Значение по умолчанию — SmoothingMode.None. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Получает и задаёт префикс имени css в svg, значение по умолчанию — пустая строка. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) Если это свойство равно true, сгенерированный svg будет подгоняться под область просмотра. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Получает или задаёт тип отображения текста, когда ширина текста превышает ширину ячейки. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Указывает качество рендеринга текста. Значение по умолчанию — TextRenderingHint.SystemDefault. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Получает или задаёт метод, используемый при преобразовании изображений в формат 1 bpp, когда [`ImageType`](../imageorprintoptions/imagetype/) установлен в Tiff и [`TiffCompression`](../imageorprintoptions/tiffcompression/) равен Ccitt3 или Ccitt4. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Получает или задаёт глубину цвета, применяемую только при сохранении страниц в формате `Tiff`. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Получает или задаёт тип сжатия, применяемый только при сохранении страниц в формате `Tiff`. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Указывает, должен ли фон сгенерированного изображения быть прозрачным. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Получает или задаёт вертикальное разрешение для сгенерированных изображений в точках на дюйм. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) Задаёт желаемую ширину и высоту изображения. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Задаёт желаемую ширину и высоту изображения. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните примерными данными для диаграммы
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Создайте столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Инициализируйте параметры изображения SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Настройте параметры рендеринга SVG
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Установите качество печати и разрешение
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Отрендерите диаграмму в SVG с настроенными параметрами
            chart.ToImage("chart_output.svg", svgOptions);

            // Продемонстрируйте интеграцию сохранения книги
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


