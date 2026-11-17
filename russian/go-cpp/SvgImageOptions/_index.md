---
title: "Класс SvgImageOptions"
linktitle: "SvgImageOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SvgImageOptions. Инкапсулирует объект, представляющий svgimageoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/svgimageoptions/
---

## SvgImageOptions class

Параметры генерации изображения Svg.

```go

type SvgImageOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSvgImageOptions](./newsvgimageoptions/) | Конструктор. |
| [NewSvgImageOptions_ImageOrPrintOptions](./newsvgimageoptions_imageorprintoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetImageType](./getimagetype/) | Получает или задаёт формат генерируемых изображений. Значение по умолчанию: PNG. |
| [SetImageType](./setimagetype/) | Получает или задаёт формат генерируемых изображений. Значение по умолчанию: PNG. |
| [GetFitToViewPort](./getfittoviewport/) | Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [SetFitToViewPort](./setfittoviewport/) | Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [GetCssPrefix](./getcssprefix/) | Получает или задаёт префикс имени css в svg, значение по умолчанию — пустая строка. |
| [SetCssPrefix](./setcssprefix/) | Получает или задаёт префикс имени css в svg, значение по умолчанию — пустая строка. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Получает или задаёт тип шрифта, встроенного в Svg. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Получает или задаёт тип шрифта, встроенного в Svg. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | Если PrintWithStatusDialog = true, будет отображён диалог, показывающий текущий статус печати; иначе такой диалог не будет показан. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | Если PrintWithStatusDialog = true, будет отображён диалог, показывающий текущий статус печати; иначе такой диалог не будет показан. |
| [GetHorizontalResolution](./gethorizontalresolution/) | Получает или задаёт горизонтальное разрешение генерируемых изображений в точках на дюйм. |
| [SetHorizontalResolution](./sethorizontalresolution/) | Получает или задаёт горизонтальное разрешение генерируемых изображений в точках на дюйм. |
| [GetVerticalResolution](./getverticalresolution/) | Получает или задаёт вертикальное разрешение генерируемых изображений в точках на дюйм. |
| [SetVerticalResolution](./setverticalresolution/) | Получает или задаёт вертикальное разрешение генерируемых изображений в точках на дюйм. |
| [GetTiffCompression](./gettiffcompression/) | Получает или задаёт тип сжатия, применяемый только при сохранении страниц в формат <c>Tiff</c>. |
| [SetTiffCompression](./settiffcompression/) | Получает или задаёт тип сжатия, применяемый только при сохранении страниц в формат <c>Tiff</c>. |
| [GetTiffColorDepth](./gettiffcolordepth/) | Получает или задаёт глубину цвета, применяемую только при сохранении страниц в формат <c>Tiff</c>. |
| [SetTiffColorDepth](./settiffcolordepth/) | Получает или задаёт глубину цвета, применяемую только при сохранении страниц в формат <c>Tiff</c>. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | Получает или задаёт метод, используемый при преобразовании изображений в формат 1 bpp, когда ImageType — Tiff и TiffCompression равно Ccitt3 или Ccitt4. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | Получает или задаёт метод, используемый при преобразовании изображений в формат 1 bpp, когда ImageType — Tiff и TiffCompression равно Ccitt3 или Ccitt4. |
| [GetPrintingPage](./getprintingpage/) | Указывает, какие страницы не будут печататься. |
| [SetPrintingPage](./setprintingpage/) | Указывает, какие страницы не будут печататься. |
| [GetQuality](./getquality/) | Получает или задаёт значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формат <c>Jpeg</c>. Значение по умолчанию — 100. |
| [SetQuality](./setquality/) | Получает или задаёт значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формат <c>Jpeg</c>. Значение по умолчанию — 100. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Если OnePagePerSheet равно true, всё содержимое листа будет выводиться на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Если OnePagePerSheet равно true, всё содержимое листа будет выводиться на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Если AllColumnsInOnePagePerSheet = true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина формата бумаги в настройках страницы станет недействительной, однако остальные параметры настройки страницы сохранят своё действие. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Если AllColumnsInOnePagePerSheet = true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина формата бумаги в настройках страницы станет недействительной, однако остальные параметры настройки страницы сохранят своё действие. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Реализует этот интерфейс, чтобы получить DrawObject и Bound при рендеринге. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Реализует этот интерфейс, чтобы получить DrawObject и Bound при рендеринге. |
| [GetOnlyArea](./getonlyarea/) | Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться. |
| [SetOnlyArea](./setonlyarea/) | Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться. |
| [GetTransparent](./gettransparent/) | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [SetTransparent](./settransparent/) | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Указывает, следует ли заменять шрифт символа только когда шрифт ячейки несовместим с ним. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Указывает, следует ли заменять шрифт символа только когда шрифт ячейки несовместим с ним. |
| [SetPageIndex](./setpageindex/) | Получает или задаёт нулевой индекс первой страницы для сохранения. |
| [GetPageIndex](./getpageindex/) | Получает или задаёт нулевой индекс первой страницы для сохранения. |
| [SetPageCount](./setpagecount/) | Получает или задаёт количество страниц для сохранения. |
| [GetPageCount](./getpagecount/) | Получает или задаёт количество страниц для сохранения. |
| [SetDesiredSize](./setdesiredsize/) | Устанавливает желаемую ширину и высоту изображения. |
| [IsOptimized](./isoptimized/) | Указывает, следует ли оптимизировать выводимые элементы. |
| [SetIsOptimized](./setisoptimized/) | Указывает, следует ли оптимизировать выводимые элементы. |
| [GetDefaultFont](./getdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. |
| [SetDefaultFont](./setdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите значение true, чтобы сначала попытаться использовать шрифт по умолчанию книги для отображения этих символов. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Когда символы в Excel являются Unicode и не заданы правильным шрифтом в стиле ячейки, они могут отображаться как блоки в pdf, изображении. Установите значение true, чтобы сначала попытаться использовать шрифт по умолчанию книги для отображения этих символов. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [GetGridlineType](./getgridlinetype/) | Получает или задаёт тип линий сетки. |
| [SetGridlineType](./setgridlinetype/) | Получает или задаёт тип линий сетки. |
| [GetGridlineColor](./getgridlinecolor/) | Получает или задает цвет линий сетки. |
| [SetGridlineColor](./setgridlinecolor/) | Получает или задает цвет линий сетки. |
| [GetTextCrossType](./gettextcrosstype/) | Получает или задаёт тип отображения текста, когда ширина текста превышает ширину ячейки. |
| [SetTextCrossType](./settextcrosstype/) | Получает или задаёт тип отображения текста, когда ширина текста превышает ширину ячейки. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Получает или задаёт язык редактирования по умолчанию. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Получает или задаёт язык редактирования по умолчанию. |
| [GetSheetSet](./getsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Получает или задаёт листы для рендеринга. По умолчанию — все видимые листы в книге: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Настройка рендеринга EMF метафайлов в исходном файле. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Настройка рендеринга EMF метафайлов в исходном файле. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Получает или задаёт пользовательские настройки во время рендеринга. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Получает или задаёт пользовательские настройки во время рендеринга. |
