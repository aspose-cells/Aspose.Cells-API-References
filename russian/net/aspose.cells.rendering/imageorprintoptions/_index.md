---
title: "Класс ImageOrPrintOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.ImageOrPrintOptions. Позволяет задавать параметры при рендеринге листа в изображения, печати листа или рендеринге диаграммы в изображение"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Позволяет задавать параметры при рендеринге листа в изображения, печати листа или рендеринге диаграммы в изображение.

```csharp
public class ImageOrPrintOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в настройках страницы будет недействительной, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Указывает тип изображения диаграммы при конвертации. значение по умолчанию: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Когда символы в Excel являются Unicode и для них не установлен корректный шрифт в стиле ячейки, они могут отображаться как блоки в PDF, изображении. Установите значение true, чтобы попытаться сначала использовать шрифт по умолчанию книги для отображения этих символов. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Клиент может выполнять специальный вывод на принтер при печати каждой страницы с использованием этого EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Клиент может управлять настройками страницы принтера при печати каждой страницы с использованием этого EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Получает или задает пользовательские настройки во время рендеринга. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Получает или задает язык редактирования по умолчанию. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Когда символы в Excel являются Unicode и для них не установлен корректный шрифт в стиле ячейки, они могут отображаться как блоки в PDF, изображении. Установите свойство DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Реализуйте этот интерфейс, чтобы получить DrawObject и Bound при рендеринге. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Указывает имя файла встроенного изображения в SVG. Это должен быть полный путь с каталогом, например "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Настройка рендеринга Emf метафайлов в исходном файле. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Получает или задает EmfType, который указывает формат Metafile. Значение по умолчанию — EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Получает или задает цвет линий сетки. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Получает или задает тип линий сетки. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Получает или задает горизонтальное разрешение генерируемых изображений в точках на дюйм. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Получает или задает формат сгенерированных изображений. значение по умолчанию: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Указывает, автоматически подгоняется ли ширина и высота ячеек под значение ячейки. Значение по умолчанию — false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Указывает, следует ли заменять шрифт символа только тогда, когда шрифт ячейки несовместим с ним. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Указывает, следует ли оптимизировать выводимые элементы. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Если параметр OnePagePerSheet установлен в true, всё содержимое одного листа будет выводиться на одну страницу в результате. Формат бумаги из настройки pagesetup будет недействительным, а остальные настройки pagesetup сохранят своё действие. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Если это свойство равно true, будет выведена одна область, и масштаб не будет применяться. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Получает или задает количество страниц для сохранения. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Получает или задает нулевой индекс первой страницы для сохранения. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Управление/индикация прогресса процесса сохранения страницы. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Получает или задает пиксельный формат генерируемых изображений. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Указывает, какие страницы не будут печататься. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Если PrintWithStatusDialog = true, будет отображён диалог, показывающий текущий статус печати. В противном случае такой диалог не будет показан. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Получает или задает значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. Значение по умолчанию — 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Получает или задает тип формата выходного файла. Поддерживает Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Получает или задает листы для рендеринга. По умолчанию — все видимые листы в рабочей книге: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Указывает, применяется ли сглаживание (антиалиасинг) к линиям и кривым и к краям заполненных областей. Значение по умолчанию — SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Получает и задает префикс имени css в svg, значение по умолчанию — пустая строка. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Указывает качество рендеринга текста. Значение по умолчанию — TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Получает или задает метод, используемый при преобразовании изображений в формат 1 bpp, когда [`ImageType`](./imagetype/) — Tiff и [`TiffCompression`](./tiffcompression/) равно Ccitt3 или Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Получает или задает глубину цвета, применяемую только при сохранении страниц в формат `Tiff`. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Получает или задает тип сжатия, применяемый только при сохранении страниц в формат `Tiff`. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Получает или задает вертикальное разрешение для сгенерированных изображений в точках на дюйм. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Задает желаемую ширину и высоту изображения. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Задает желаемую ширину и высоту изображения. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создайте ImageOrPrintOptions и задайте свойства
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Создайте новую рабочую книгу с примерными данными и диаграммой
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Сохраните диаграмму как изображение, используя параметры
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


