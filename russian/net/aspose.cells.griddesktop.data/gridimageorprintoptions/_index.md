---
title: "Класс GridImageOrPrintOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions. Позволяет задавать параметры при рендеринге worksheet в изображения, печати worksheet или рендеринге chart в изображение"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Позволяет задавать параметры при рендеринге листа в изображения, печати листа или рендеринге диаграммы в изображение.

```csharp
public class GridImageOrPrintOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | Конструктор GridImageOrPrintOptions |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в настройках страницы будет недействительной, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Когда символы в Excel являются Unicode и для них не установлен корректный шрифт в стиле ячейки, они могут отображаться как блоки в PDF, изображении. Установите значение true, чтобы попытаться сначала использовать шрифт по умолчанию книги для отображения этих символов. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | Когда символы в Excel являются Unicode и для них не установлен корректный шрифт в стиле ячейки, они могут отображаться как блоки в PDF, изображении. Установите свойство DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Указывает имя файла встроенного изображения в svg. Это должен быть полный путь с каталогом, например "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Получает или задает EmfType, который указывает формат Metafile. Значение по умолчанию — EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Получает или задает тип линий сетки. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Получает или задает горизонтальное разрешение генерируемых изображений в точках на дюйм. Применяется к методу генерации изображения, за исключением изображений формата Emf. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Получает или задает формат сгенерированных изображений. значение по умолчанию: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Указывает, следует ли заменять шрифт символа только тогда, когда шрифт ячейки несовместим с ним. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Указывает, следует ли оптимизировать выводимые элементы. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | Если параметр OnePagePerSheet установлен в true, всё содержимое одного листа будет выводиться на одну страницу в результате. Формат бумаги из настройки pagesetup будет недействительным, а остальные настройки pagesetup сохранят своё действие. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Если это свойство равно true, будет выведена одна область, и масштаб не будет применяться. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Получает или задает количество страниц для сохранения. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Получает или задает нулевой индекс первой страницы для сохранения. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Получает или задает пиксельный формат генерируемых изображений. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Указывает, какие страницы не будут печататься. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | Если PrintWithStatusDialog = true, будет отображён диалог, показывающий текущий статус печати. В противном случае такой диалог не будет показан. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Получает или задает значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. Значение по умолчанию — 100 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Указывает, применяется ли сглаживание (антиалиасинг) к линиям и кривым и к краям заполненных областей. Значение по умолчанию — SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Если это свойство равно true, сгенерированный SVG будет подгоняться под область просмотра. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Указывает качество рендеринга текста. Значение по умолчанию — TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Получает или задает вертикальное разрешение генерируемых изображений в точках на дюйм. Применяется к методу генерации изображения, за исключением изображений формата Emf. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Задает желаемую ширину и высоту изображения. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | Устанавливает листы для рендеринга. По умолчанию — все видимые листы в рабочей книге. Индексы листов начинаются с нуля. |

### См. также

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


