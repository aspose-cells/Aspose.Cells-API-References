---
title: "SvgImageOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры генерации SVG‑изображения."
type: docs
url: /ru/java/com.aspose.cells/svgimageoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
```
public class SvgImageOptions extends ImageOrPrintOptions
```

Параметры генерации SVG‑изображения.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SvgImageOptions()](#SvgImageOptions--) | Конструктор. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. |
| [getChartImageType()](#getChartImageType--) | Укажите тип изображения диаграммы при конвертации. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [getClass()](#getClass--) |  |
| [getCssPrefix()](#getCssPrefix--) | Получает префикс имени css в svg, значение по умолчанию — пустая строка. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Получает пользовательские настройки во время рендеринга. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Получает язык редактирования по умолчанию. |
| [getDefaultFont()](#getDefaultFont--) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Получает тип шрифта, встроенного в Svg. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Укажите имя файла встроенного изображения в svg. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Настройка рендеринга Emf метафайлов в исходном файле. |
| [getFitToViewPort()](#getFitToViewPort--) | Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [getGridlineColor()](#getGridlineColor--) | Получает цвет линий сетки. |
| [getGridlineType()](#getGridlineType--) | Получает тип линий сетки. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Получает горизонтальное разрешение сгенерированных изображений в точках на дюйм. |
| [getImageType()](#getImageType--) | Получает формат сгенерированных изображений. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. |
| [getOnlyArea()](#getOnlyArea--) | Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [getPageCount()](#getPageCount--) | Получает количество страниц для сохранения. |
| [getPageIndex()](#getPageIndex--) | Получает индекс первой страницы для сохранения, начиная с 0. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Контролировать/Указывать прогресс процесса сохранения страниц. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | Если PrintWithStatusDialog = true, появится диалог, показывающий текущий статус печати. |
| [getPrintingPage()](#getPrintingPage--) | Указывает, какие страницы не будут печататься. |
| [getQuality()](#getQuality--) | Получает значение, определяющее качество сгенерированных изображений, применяемое только при сохранении страниц в формат `Jpeg`. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [getSaveFormat()](#getSaveFormat--) | Получает тип формата выходного файла, поддерживает Tiff/XPS. |
| [getSheetSet()](#getSheetSet--) | Получает листы для рендеринга. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Получает префикс имени css в svg, значение по умолчанию — пустая строка. |
| [getTextCrossType()](#getTextCrossType--) | Получает тип отображаемого текста, когда ширина текста превышает ширину ячейки. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Получает глубину цвета, применяемую только при сохранении страниц в формат `Tiff`. |
| [getTiffCompression()](#getTiffCompression--) | Получает тип сжатия, применяемый только при сохранении страниц в формат `Tiff`. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Получает тип PhotometricInterpretation, применяемый только при сохранении страниц в формат `Tiff`. |
| [getTransparent()](#getTransparent--) | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [getVerticalResolution()](#getVerticalResolution--) | Получает вертикальное разрешение сгенерированных изображений в точках на дюйм. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Указывает, автоматически ли подгоняется ширина и высота ячеек по значению ячейки. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним. |
| [isOptimized()](#isOptimized--) | Указывает, следует ли оптимизировать выходные элементы. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Если AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Указывает, автоматически ли подгоняется ширина и высота ячеек по значению ячейки. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Укажите тип изображения диаграммы при конвертации. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [setCssPrefix(String value)](#setCssPrefix-java.lang.String-) | Устанавливает префикс имени css в svg, значение по умолчанию — пустая строка. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Устанавливает пользовательские параметры во время рендеринга. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Устанавливает язык редактирования по умолчанию. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf,image. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Устанавливает желаемую ширину и высоту изображения. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Устанавливает желаемую ширину и высоту изображения. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Устанавливает тип шрифта, встроенного в Svg. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Укажите имя файла встроенного изображения в svg. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Настройка рендеринга Emf метафайлов в исходном файле. |
| [setFitToViewPort(boolean value)](#setFitToViewPort-boolean-) | Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Устанавливает цвет линий сетки. |
| [setGridlineType(int value)](#setGridlineType-int-) | Устанавливает тип линий сетки. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Устанавливает горизонтальное разрешение генерируемых изображений в точках на дюйм. |
| [setImageType(int value)](#setImageType-int-) | Устанавливает формат генерируемых изображений. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Указывает, следует ли оптимизировать выходные элементы. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Указывает, следует ли выводить пустую страницу, когда нечего печатать. |
| [setPageCount(int value)](#setPageCount-int-) | Устанавливает количество страниц для сохранения. |
| [setPageIndex(int value)](#setPageIndex-int-) | Устанавливает нулевой индекс первой страницы для сохранения. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Контролировать/Указывать прогресс процесса сохранения страниц. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | Если PrintWithStatusDialog = true, появится диалог, показывающий текущий статус печати. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Указывает, какие страницы не будут печататься. |
| [setQuality(int value)](#setQuality-int-) | Устанавливает значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Устанавливает значение отдельного предпочтения для алгоритмов рендеринга. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Устанавливает тип формата выходного файла. Поддержка Tiff/XPS. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Устанавливает листы для рендеринга. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Устанавливает префикс имени css в svg, значение по умолчанию — пустая строка. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Устанавливает тип отображаемого текста, когда ширина текста превышает ширину ячейки. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Устанавливает глубину цвета, применяемую только при сохранении страниц в формате `Tiff`. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Устанавливает тип сжатия, применяемый только при сохранении страниц в формате `Tiff`. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Устанавливает тип PhotometricInterpretation, применяемый только при сохранении страниц в формате `Tiff`. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Указывает, должен ли фон сгенерированного изображения быть прозрачным. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Устанавливает вертикальное разрешение генерируемых изображений в точках на дюйм. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgImageOptions() {#SvgImageOptions--}
```
public SvgImageOptions()
```


Конструктор.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Если AllColumnsInOnePagePerSheet = true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина формата бумаги в pagesetup станет недействительной, а остальные настройки pagesetup по‑прежнему будут применяться.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Укажите тип изображения диаграммы при конвертации. значение по умолчанию: PNG.

**Remarks**

NOTE: Этот член теперь устарел. Вместо этого Chart и Shape всегда рендерятся как векторные элементы (например, точка, линия) для обеспечения качества рендеринга. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите значение true, чтобы попытаться использовать шрифт по умолчанию книги для отображения этих символов.

**Remarks**

По умолчанию — true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssPrefix() {#getCssPrefix--}
```
public String getCssPrefix()
```


Получает префикс имени css в svg, значение по умолчанию — пустая строка.

**Returns:**
java.lang.String
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Получает пользовательские настройки во время рендеринга.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Получает язык редактирования по умолчанию.

См. [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Это может отображать/рендерить разные макеты абзацев текста при установленном различном языке редактирования. По умолчанию — [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Получает тип шрифта, встроенного в Svg.

См. [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Значение по умолчанию — [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE), что указывает на то, что шрифт не будет встраиваться в Svg.

**Returns:**
int
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Укажите имя файла встроенного изображения в svg. Это должен быть полный путь с каталогом, например "c:\\\\xpsEmbedded"

**Remarks**

NOTE: Этот член теперь устарел. Вместо этого удалите это свойство, поскольку изображения теперь всегда встраиваются в Svg в формате base64. Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Настройка рендеринга Emf метафайлов в исходном файле.

См. [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Метaфайлы EMF, идентифицированные как "EMF+ Dual", могут содержать как записи EMF+, так и записи EMF. Любой тип записей может использоваться для рендеринга изображения, только записи EMF+ или только записи EMF. Когда установлен [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), при рендеринге изображения будут обрабатываться записи EMF+. В противном случае будут обрабатываться только записи EMF. Значение по умолчанию — [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Для фреймворков, зависящих от .NET System.Drawing.Common, эта настройка игнорируется.

**Returns:**
int
### getFitToViewPort() {#getFitToViewPort--}
```
public boolean getFitToViewPort()
```


Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Получает цвет линий сетки.

**Remarks**

Он будет игнорировать настройки цвета линий сетки в исходном файле.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Получает тип линий сетки.

См. [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

По умолчанию — тип Dotted.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Получает горизонтальное разрешение сгенерированных изображений в точках на дюйм.

**Remarks**

Значение по умолчанию — 96. Настройка  и  влияет на ширину и высоту выходного изображения в пикселях.

**Example**

Следующий код устанавливает разрешение 192, ширина и высота сгенерированного изображения вдвое больше, чем при разрешении, оставленном по умолчанию 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Получает формат генерируемых изображений. значение по умолчанию: PNG.

См. [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Указывает, следует ли выводить пустую страницу, когда нечего печатать.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Получает количество страниц для сохранения.

**Remarks**

Значение по умолчанию — System.Int32.MaxValue, что означает, что будут отрисованы все страницы.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Получает индекс первой страницы для сохранения, начиная с 0.

**Remarks**

По умолчанию 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Контролировать/Указывать прогресс процесса сохранения страниц.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


Если PrintWithStatusDialog = true, появится диалог, показывающий текущий статус печати. иначе такой диалог не будет отображаться.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Указывает, какие страницы не будут печататься.

См. [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Получает значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. Значение по умолчанию — 100.

**Remarks**

Имеет эффект только при сохранении в JPEG. Значение должно быть от 0 до 100. Значение по умолчанию — 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает тип формата выходного файла, поддерживает Tiff/XPS.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него для Tiff/Svg используйте [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); для Xps — [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) с [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Это свойство будет удалено через 12 месяцев, начиная с августа 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Получает листы для рендеринга. По умолчанию — все видимые листы в рабочей книге: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Набор игнорируется, когда используется в [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Получает префикс имени css в svg, значение по умолчанию — пустая строка.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Получает тип отображаемого текста, когда ширина текста превышает ширину ячейки.

См. [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Получает глубину цвета, применяемую только при сохранении страниц в формат `Tiff`.

Смотрите [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Имеет эффект только при сохранении в TIFF. Если TiffCompression установлен в CCITT3 или CCITT4, это не сработает, глубина цвета генерируемого tiff‑изображения всегда будет 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Получает тип сжатия, применяемый только при сохранении страниц в формат `Tiff`.

Смотрите [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Имеет эффект только при сохранении в TIFF. Значение по умолчанию — Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


Получает тип PhotometricInterpretation, применяемый только при сохранении страниц в формат `Tiff`.

**Remarks**

Имеет эффект только при сохранении в TIFF. Значение по умолчанию — -1, что означает отсутствие применения PhotometricInterpretation.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Указывает, должен ли фон сгенерированного изображения быть прозрачным.

**Remarks**

Значение по умолчанию — false. Это означает, что фон генерируемых изображений белый.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Получает вертикальное разрешение сгенерированных изображений в точках на дюйм.

**Remarks**

Значение по умолчанию — 96. Настройка  и  влияет на ширину и высоту выходного изображения в пикселях.

**Example**

Следующий код устанавливает разрешение 192, ширина и высота сгенерированного изображения вдвое больше, чем при разрешении, оставленном по умолчанию 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Получает обратный вызов предупреждения.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Указывает, автоматически ли подгоняется ширина и высота ячеек по значению ячейки. Значение по умолчанию — false.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него это свойство не используется, пожалуйста, удалите это свойство. Это свойство будет удалено через 12 месяцев, начиная с августа 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним.

**Remarks**

По умолчанию false. Сначала будет использован шрифт по умолчанию из Workbook и PdfSaveOption/system для шрифта ячеек.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Указывает, следует ли оптимизировать выходные элементы.

**Remarks**

Значение по умолчанию — false. В настоящее время, когда это свойство установлено в true, выполняются следующие оптимизации: 1. оптимизация границ линий. 2. оптимизация размера файла при рендеринге в изображение Svg.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Если AllColumnsInOnePagePerSheet = true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина формата бумаги в pagesetup станет недействительной, а остальные настройки pagesetup по‑прежнему будут применяться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Указывает, автоматически ли подгоняется ширина и высота ячеек по значению ячейки. Значение по умолчанию — false.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него это свойство не используется, пожалуйста, удалите это свойство. Это свойство будет удалено через 12 месяцев, начиная с августа 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Укажите тип изображения диаграммы при конвертации. значение по умолчанию: PNG.

**Remarks**

NOTE: Этот член теперь устарел. Вместо этого Chart и Shape всегда рендерятся как векторные элементы (например, точка, линия) для обеспечения качества рендеринга. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите значение true, чтобы попытаться использовать шрифт по умолчанию книги для отображения этих символов.

**Remarks**

По умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCssPrefix(String value) {#setCssPrefix-java.lang.String-}
```
public void setCssPrefix(String value)
```


Устанавливает префикс имени css в svg, значение по умолчанию — пустая строка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Устанавливает пользовательские параметры во время рендеринга.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Устанавливает язык редактирования по умолчанию.

См. [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Это может отображать/рендерить разные макеты абзацев текста при установленном различном языке редактирования. По умолчанию — [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Если символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в PDF или изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Устанавливает желаемую ширину и высоту изображения.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) задав параметр keepAspectRatio в false. Это свойство будет удалено через 12 месяцев, начиная с мая 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredWidth | int | желаемая ширина в пикселях |
| desiredHeight | int | желаемая высота в пикселях |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Устанавливает желаемую ширину и высоту изображения.

**Remarks**

Ширина и высота выходного изображения в пикселях будут определяться только установленными желаемыми шириной и высотой.  и  не будут влиять на ширину и высоту выходного изображения в этом случае.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| desiredWidth | int | желаемая ширина в пикселях |
| desiredHeight | int | желаемая высота в пикселях |
| keepAspectRatio | boolean | нужно ли сохранять соотношение сторон исходного изображения |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Реализует этот интерфейс для получения DrawObject и Bound при рендеринге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Устанавливает тип шрифта, встроенного в Svg.

См. [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Значение по умолчанию — [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE), что указывает на то, что шрифт не будет встраиваться в Svg.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Укажите имя файла встроенного изображения в svg. Это должен быть полный путь с каталогом, например "c:\\\\xpsEmbedded"

**Remarks**

NOTE: Этот член теперь устарел. Вместо этого удалите это свойство, поскольку изображения теперь всегда встраиваются в Svg в формате base64. Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Настройка рендеринга Emf метафайлов в исходном файле.

См. [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Метaфайлы EMF, идентифицированные как "EMF+ Dual", могут содержать как записи EMF+, так и записи EMF. Любой тип записей может использоваться для рендеринга изображения, только записи EMF+ или только записи EMF. Когда установлен [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), при рендеринге изображения будут обрабатываться записи EMF+. В противном случае будут обрабатываться только записи EMF. Значение по умолчанию — [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Для фреймворков, зависящих от .NET System.Drawing.Common, эта настройка игнорируется.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFitToViewPort(boolean value) {#setFitToViewPort-boolean-}
```
public void setFitToViewPort(boolean value)
```


Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Указывает, следует ли заменять шрифт символа только в случае, когда шрифт ячейки не совместим с ним.

**Remarks**

По умолчанию false. Сначала будет использован шрифт по умолчанию из Workbook и PdfSaveOption/system для шрифта ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Устанавливает цвет линий сетки.

**Remarks**

Он будет игнорировать настройки цвета линий сетки в исходном файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Устанавливает тип линий сетки.

См. [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

По умолчанию — тип Dotted.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Устанавливает горизонтальное разрешение генерируемых изображений в точках на дюйм.

**Remarks**

Значение по умолчанию — 96. Настройка  и  влияет на ширину и высоту выходного изображения в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Устанавливает формат генерируемых изображений. значение по умолчанию: PNG.

См. [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Если OnePagePerSheet равно true, всё содержимое одного листа будет выводиться только на одну страницу в результате. Размер бумаги в pagesetup будет недействительным, а остальные настройки pagesetup по‑прежнему будут применяться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Указывает, следует ли оптимизировать выходные элементы.

**Remarks**

Значение по умолчанию — false. В настоящее время, когда это свойство установлено в true, выполняются следующие оптимизации: 1. оптимизация границ линий. 2. оптимизация размера файла при рендеринге в изображение Svg.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Указывает, следует ли выводить пустую страницу, когда нечего печатать.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Устанавливает количество страниц для сохранения.

**Remarks**

Значение по умолчанию — System.Int32.MaxValue, что означает, что будут отрисованы все страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Устанавливает нулевой индекс первой страницы для сохранения.

**Remarks**

По умолчанию 0.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Контролировать/Указывать прогресс процесса сохранения страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


Если PrintWithStatusDialog = true, появится диалог, показывающий текущий статус печати. иначе такой диалог не будет отображаться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Указывает, какие страницы не будут печататься.

См. [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Устанавливает значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. Значение по умолчанию — 100.

**Remarks**

Имеет эффект только при сохранении в JPEG. Значение должно быть от 0 до 100. Значение по умолчанию — 100.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Устанавливает значение отдельного параметра для алгоритмов рендеринга. Категории подсказок включают элементы управления качеством рендеринга и общим компромиссом между временем и качеством в процессе рендеринга. Обратитесь к классу RenderingHints для определения некоторых общих ключей и значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ключ | java.awt.RenderingHints.Key | ключ подсказки, который будет установлен. |
| значение | java.lang.Object | значение, указывающее предпочтения для указанной категории подсказки. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


Если это свойство истинно, сгенерированный svg будет подгоняться под область просмотра.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Устанавливает тип формата выходного файла. Поддержка Tiff/XPS.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него для Tiff/Svg используйте [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); для Xps — [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) с [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Это свойство будет удалено через 12 месяцев, начиная с августа 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Устанавливает листы для отображения. По умолчанию — все видимые листы в рабочей книге: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Набор игнорируется, когда используется в [SheetRender](../../com.aspose.cells/sheetrender).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Устанавливает префикс имени css в svg, значение по умолчанию — пустая строка.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Устанавливает тип отображаемого текста, когда ширина текста превышает ширину ячейки.

См. [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Устанавливает глубину цвета, применяемую только при сохранении страниц в формате `Tiff`.

Смотрите [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Имеет эффект только при сохранении в TIFF. Если TiffCompression установлен в CCITT3 или CCITT4, это не сработает, глубина цвета генерируемого tiff‑изображения всегда будет 1.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Устанавливает тип сжатия, применяемый только при сохранении страниц в формате `Tiff`.

Смотрите [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Имеет эффект только при сохранении в TIFF. Значение по умолчанию — Lzw.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Устанавливает тип PhotometricInterpretation, применяемый только при сохранении страниц в формате `Tiff`.

**Remarks**

Имеет эффект только при сохранении в TIFF. Значение по умолчанию — -1, что означает отсутствие применения PhotometricInterpretation.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Указывает, должен ли фон сгенерированного изображения быть прозрачным.

**Remarks**

Значение по умолчанию — false. Это означает, что фон генерируемых изображений белый.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Устанавливает вертикальное разрешение генерируемых изображений в точках на дюйм.

**Remarks**

Значение по умолчанию — 96. Настройка  и  влияет на ширину и высоту выходного изображения в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Устанавливает обратный вызов предупреждения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

