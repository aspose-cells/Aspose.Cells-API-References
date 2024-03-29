---
title: ImageOrPrintOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Позволяет указать параметры при рендеринге рабочего листа в изображения печати рабочего листа или рендеринге диаграммы в изображение.
type: docs
weight: 5140
url: /ru/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Позволяет указать параметры при рендеринге рабочего листа в изображения, печати рабочего листа или рендеринге диаграммы в изображение.

```csharp
public class ImageOrPrintOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | Если AllColumnsInOnePagePerSheet имеет значение true , все содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в pagesetup будет недействительной, а другие настройки pagesetup останутся в силе. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | Если символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки, Они могут отображаться в виде блока в pdf, image. Установите для этого параметра значение true, чтобы попытаться использовать шрифт рабочей книги по умолчанию для отображения этих символов в первую очередь. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | Клиент может специально выводить на принтер при печати каждой страницы с помощью этого EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | Клиент может управлять настройкой страницы принтера при печати каждой страницы с помощью этого EventHandler |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Получает или устанавливает язык редактирования по умолчанию. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | Если символы в Excel имеют формат Unicode и для них не задан правильный шрифт в стиле ячейки, Они могут отображаться в виде блока в pdf, image. Установите шрифт по умолчанию, например MingLiu или MS Gothic, для отображения этих символов. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих символов Юникода. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | Указывает имя файла встроенного изображения в svg. Это должен быть полный путь с каталогом вида "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Получает или задает EmfType, указывающий формат метафайла.. Значение по умолчанию — EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Получает или задает тип линии сетки. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Получает или задает разрешение по горизонтали для сгенерированных изображений в точках на дюйм. Применяет метод создания изображения, за исключением изображений в формате Emf. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Получает или задает формат сгенерированных изображений. значение по умолчанию: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Указывает, подгоняются ли ширина и высота ячеек автоматически по значению ячейки. Значение по умолчанию — false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Указывает, следует ли заменять шрифт символа только в том случае, если шрифт ячейки несовместим с ним. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Указывает, следует ли оптимизировать элементы вывода. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | Если OnePagePerSheet имеет значение true , все содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недопустимым, а другие настройки pagesetup по-прежнему будут действовать. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Если это свойство имеет значение true , будет выведена одна область, и масштаб не будет действовать. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Указывает, выводить ли пустую страницу, когда нечего печатать. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Получает или задает количество страниц для сохранения. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Получает или задает отсчитываемый от 0 индекс первой страницы для сохранения. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Управление/указание хода процесса сохранения страницы. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Получает или задает формат пикселей для сгенерированных изображений. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Указывает, какие страницы не будут напечатаны. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | Если PrintWithStatusDialog = true , появится диалоговое окно, показывающее текущее состояние печати. иначе такое диалоговое окно не будет отображаться. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Получает или задает значение, определяющее качество сгенерированных изображений для применения только при сохранении страниц в`JPEG` формат. Значение по умолчанию: 100 . |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Получает или задает формат выходного файла type Support Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Указывает, применяется ли сглаживание (сглаживание) к линиям, кривым и краям заполненных областей. Значение по умолчанию — SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | если это свойство истинно, сгенерированный svg будет соответствовать порту просмотра. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Получает или задает отображаемый тип текста, когда ширина текста больше ширины ячейки. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Определяет качество рендеринга текста. Значение по умолчанию — TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Получает или задает разрядность, которая применяется только при сохранении страниц в`размолвка` формат. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Получает или задает тип сжатия, применяемый только при сохранении страниц в`размолвка` формат. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Получает или задает разрешение по вертикали для сгенерированных изображений в точках на дюйм. Применяет метод создания изображения, за исключением изображения в формате Emf. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Устанавливает желаемую ширину и высоту изображения. |

### Примеры

```csharp

[C#]

//Установить параметры изображения или печати
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Устанавливаем формат выходного изображения
options.ImageType = ImageType.Png;

//Установить горизонтальное разрешение
options.HorizontalResolution = 300;

//Установить вертикальное разрешение
options.VerticalResolution = 300;

//Создать экземпляр рабочей книги
Workbook book = new Workbook("test.xls");

// Сохраняем диаграмму как изображение, используя параметры ImageOrPrint
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Установите параметры изображения или печати
Dim options As New ImageOrPrintOptions()

'Установить формат выходного изображения
options.ImageType = ImageType.Png

'Установить горизонтальное разрешение
options.HorizontalResolution = 300

'Установить вертикальное разрешение
options.VerticalResolution = 300

'Создание рабочей книги
Dim book As New Workbook("test.xls")

'Сохранить диаграмму как изображение с помощью параметров ImageOrPrint
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Смотрите также

* пространство имен [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
