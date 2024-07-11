---
title: ImageOrPrintOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.
type: docs
url: /nodejs-cpp/imageorprintoptions/
---

## ImageOrPrintOptions class

Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.

```javascript
class ImageOrPrintOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [setPrintWithStatusDialog(boolean)](#setPrintWithStatusDialog-boolean-)| If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--)| If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [getHorizontalResolution()](#getHorizontalResolution--)| Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. |
| [setHorizontalResolution(number)](#setHorizontalResolution-number-)| Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. |
| [getVerticalResolution()](#getVerticalResolution--)| Gets or sets the vertical  resolution for generated images, in dots per inch. Applies generating image method except Emf format image. |
| [setVerticalResolution(number)](#setVerticalResolution-number-)| Gets or sets the vertical  resolution for generated images, in dots per inch. Applies generating image method except Emf format image. |
| [getTiffCompression()](#getTiffCompression--)| Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
| [setTiffCompression(TiffCompression)](#setTiffCompression-tiffcompression-)| Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
| [getTiffColorDepth()](#getTiffColorDepth--)| Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
| [setTiffColorDepth(ColorDepth)](#setTiffColorDepth-colordepth-)| Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
| [getTiffBinarizationMethod()](#getTiffBinarizationMethod--)| Gets or sets method used while converting images to 1 bpp format when [ImageType](./imagetype/) is Tiff and [ImageType](./imagetype/) is equal to Ccitt3 or Ccitt4. |
| [setTiffBinarizationMethod(ImageBinarizationMethod)](#setTiffBinarizationMethod-imagebinarizationmethod-)| Gets or sets method used while converting images to 1 bpp format when [ImageType](./imagetype/) is Tiff and [ImageType](./imagetype/) is equal to Ccitt3 or Ccitt4. |
| [getPrintingPage()](#getPrintingPage--)| Indicates which pages will not be printed. |
| [setPrintingPage(PrintingPageType)](#setPrintingPage-printingpagetype-)| Indicates which pages will not be printed. |
| [getQuality()](#getQuality--)| Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
| [setQuality(number)](#setQuality-number-)| Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
| [getImageType()](#getImageType--)| Gets or sets the format of the generated images. default value: PNG. |
| [setImageType(ImageType)](#setImageType-imagetype-)| Gets or sets the format of the generated images. default value: PNG. |
| [getOnePagePerSheet()](#getOnePagePerSheet--)| If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [setOnePagePerSheet(boolean)](#setOnePagePerSheet-boolean-)| If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--)| If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [setAllColumnsInOnePagePerSheet(boolean)](#setAllColumnsInOnePagePerSheet-boolean-)| If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--)| Implements this interface to get DrawObject and Bound when rendering. |
| [setDrawObjectEventHandler(DrawObjectEventHandler)](#setDrawObjectEventHandler-drawobjecteventhandler-)| Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--)| Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [setEmbededImageNameInSvg(string)](#setEmbededImageNameInSvg-string-)| Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--)| if this property is true, the generated svg will fit to view port. |
| [setSVGFitToViewPort(boolean)](#setSVGFitToViewPort-boolean-)| if this property is true, the generated svg will fit to view port. |
| [getOnlyArea()](#getOnlyArea--)| If this property is true , one Area will be output, and no scale will take effect. |
| [setOnlyArea(boolean)](#setOnlyArea-boolean-)| If this property is true , one Area will be output, and no scale will take effect. |
| [getTransparent()](#getTransparent--)| Indicates if the background of generated image should be transparent. |
| [setTransparent(boolean)](#setTransparent-boolean-)| Indicates if the background of generated image should be transparent. |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| Gets or sets warning callback. |
| [getPageSavingCallback()](#getPageSavingCallback--)| Control/Indicate progress of page saving process. |
| [setPageSavingCallback(IPageSavingCallback)](#setPageSavingCallback-ipagesavingcallback-)| Control/Indicate progress of page saving process. |
| [setIsFontSubstitutionCharGranularity(boolean)](#setIsFontSubstitutionCharGranularity-boolean-)| Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--)| Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [setPageIndex(number)](#setPageIndex-number-)| Gets or sets the 0-based index of the first page to save. |
| [getPageIndex()](#getPageIndex--)| Gets or sets the 0-based index of the first page to save. |
| [setPageCount(number)](#setPageCount-number-)| Gets or sets the number of pages to save. |
| [getPageCount()](#getPageCount--)| Gets or sets the number of pages to save. |
| [isOptimized()](#isOptimized--)| Indicates whether to optimize the output elements. |
| [setIsOptimized(boolean)](#setIsOptimized-boolean-)| Indicates whether to optimize the output elements. |
| [getDefaultFont()](#getDefaultFont--)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [setDefaultFont(string)](#setDefaultFont-string-)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [setCheckWorkbookDefaultFont(boolean)](#setCheckWorkbookDefaultFont-boolean-)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--)| Indicates whether to output a blank page when there is nothing to print. |
| [setOutputBlankPageWhenNothingToPrint(boolean)](#setOutputBlankPageWhenNothingToPrint-boolean-)| Indicates whether to output a blank page when there is nothing to print. |
| [getGridlineType()](#getGridlineType--)| Gets or sets gridline type. |
| [setGridlineType(GridlineType)](#setGridlineType-gridlinetype-)| Gets or sets gridline type. |
| [getTextCrossType()](#getTextCrossType--)| Gets or sets displaying text type when the text width is larger than cell width. |
| [setTextCrossType(TextCrossType)](#setTextCrossType-textcrosstype-)| Gets or sets displaying text type when the text width is larger than cell width. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--)| Gets or sets default edit language. |
| [setDefaultEditLanguage(DefaultEditLanguage)](#setDefaultEditLanguage-defaulteditlanguage-)| Gets or sets default edit language. |
| [getSheetSet()](#getSheetSet--)| Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](./aspose.cells.rendering.sheetset.visible/). |
| [setSheetSet(SheetSet)](#setSheetSet-sheetset-)| Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](./aspose.cells.rendering.sheetset.visible/). |
| [getEmfRenderSetting()](#getEmfRenderSetting--)| Setting for rendering Emf metafile. |
| [setEmfRenderSetting(EmfRenderSetting)](#setEmfRenderSetting-emfrendersetting-)| Setting for rendering Emf metafile. |
| [setDesiredSize(number, number, boolean)](#setDesiredSize-number-number-boolean-)| Sets desired width and height of image. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### setPrintWithStatusDialog(boolean) {#setPrintWithStatusDialog-boolean-}

If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

```javascript
setPrintWithStatusDialog(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}

If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

```javascript
getPrintWithStatusDialog() : boolean;
```


### getHorizontalResolution() {#getHorizontalResolution--}

Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images.

```javascript
getHorizontalResolution() : number;
```


**Remarks**

The default value is 96.

### setHorizontalResolution(number) {#setHorizontalResolution-number-}

Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images.

```javascript
setHorizontalResolution(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The default value is 96.

### getVerticalResolution() {#getVerticalResolution--}

Gets or sets the vertical  resolution for generated images, in dots per inch. Applies generating image method except Emf format image.

```javascript
getVerticalResolution() : number;
```


**Remarks**

The default value is 96.

### setVerticalResolution(number) {#setVerticalResolution-number-}

Gets or sets the vertical  resolution for generated images, in dots per inch. Applies generating image method except Emf format image.

```javascript
setVerticalResolution(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The default value is 96.

### getTiffCompression() {#getTiffCompression--}

Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format.

```javascript
getTiffCompression() : TiffCompression;
```


**Returns**

[TiffCompression](./tiffcompression/)

**Remarks**

Has effect only when saving to TIFF. The default value is Lzw.

### setTiffCompression(TiffCompression) {#setTiffCompression-tiffcompression-}

Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format.

```javascript
setTiffCompression(value: TiffCompression) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TiffCompression](./tiffcompression/) | The value to set. |

**Remarks**

Has effect only when saving to TIFF. The default value is Lzw.

### getTiffColorDepth() {#getTiffColorDepth--}

Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format.

```javascript
getTiffColorDepth() : ColorDepth;
```


**Returns**

[ColorDepth](./colordepth/)

**Remarks**

Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### setTiffColorDepth(ColorDepth) {#setTiffColorDepth-colordepth-}

Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format.

```javascript
setTiffColorDepth(value: ColorDepth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ColorDepth](./colordepth/) | The value to set. |

**Remarks**

Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### getTiffBinarizationMethod() {#getTiffBinarizationMethod--}

Gets or sets method used while converting images to 1 bpp format when [ImageType](./imagetype/) is Tiff and [ImageType](./imagetype/) is equal to Ccitt3 or Ccitt4.

```javascript
getTiffBinarizationMethod() : ImageBinarizationMethod;
```


**Returns**

[ImageBinarizationMethod](./imagebinarizationmethod/)

**Remarks**

The default value is FloydSteinbergDithering.

### setTiffBinarizationMethod(ImageBinarizationMethod) {#setTiffBinarizationMethod-imagebinarizationmethod-}

Gets or sets method used while converting images to 1 bpp format when [ImageType](./imagetype/) is Tiff and [ImageType](./imagetype/) is equal to Ccitt3 or Ccitt4.

```javascript
setTiffBinarizationMethod(value: ImageBinarizationMethod) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageBinarizationMethod](./imagebinarizationmethod/) | The value to set. |

**Remarks**

The default value is FloydSteinbergDithering.

### getPrintingPage() {#getPrintingPage--}

Indicates which pages will not be printed.

```javascript
getPrintingPage() : PrintingPageType;
```


**Returns**

[PrintingPageType](./printingpagetype/)

### setPrintingPage(PrintingPageType) {#setPrintingPage-printingpagetype-}

Indicates which pages will not be printed.

```javascript
setPrintingPage(value: PrintingPageType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintingPageType](./printingpagetype/) | The value to set. |

### getQuality() {#getQuality--}

Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100

```javascript
getQuality() : number;
```


**Remarks**

Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### setQuality(number) {#setQuality-number-}

Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100

```javascript
setQuality(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### getImageType() {#getImageType--}

Gets or sets the format of the generated images. default value: PNG.

```javascript
getImageType() : ImageType;
```


**Returns**

[ImageType](./imagetype/)

### setImageType(ImageType) {#setImageType-imagetype-}

Gets or sets the format of the generated images. default value: PNG.

```javascript
setImageType(value: ImageType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageType](./imagetype/) | The value to set. |

### getOnePagePerSheet() {#getOnePagePerSheet--}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
getOnePagePerSheet() : boolean;
```


### setOnePagePerSheet(boolean) {#setOnePagePerSheet-boolean-}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
setOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
getAllColumnsInOnePagePerSheet() : boolean;
```


### setAllColumnsInOnePagePerSheet(boolean) {#setAllColumnsInOnePagePerSheet-boolean-}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
setAllColumnsInOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}

Implements this interface to get DrawObject and Bound when rendering.

```javascript
getDrawObjectEventHandler() : DrawObjectEventHandler;
```


**Returns**

[DrawObjectEventHandler](./drawobjecteventhandler/)

### setDrawObjectEventHandler(DrawObjectEventHandler) {#setDrawObjectEventHandler-drawobjecteventhandler-}

Implements this interface to get DrawObject and Bound when rendering.

```javascript
setDrawObjectEventHandler(value: DrawObjectEventHandler) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](./drawobjecteventhandler/) | The value to set. |

### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}

Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"

```javascript
getEmbededImageNameInSvg() : string;
```


### setEmbededImageNameInSvg(string) {#setEmbededImageNameInSvg-string-}

Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"

```javascript
setEmbededImageNameInSvg(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSVGFitToViewPort() {#getSVGFitToViewPort--}

if this property is true, the generated svg will fit to view port.

```javascript
getSVGFitToViewPort() : boolean;
```


### setSVGFitToViewPort(boolean) {#setSVGFitToViewPort-boolean-}

if this property is true, the generated svg will fit to view port.

```javascript
setSVGFitToViewPort(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOnlyArea() {#getOnlyArea--}

If this property is true , one Area will be output, and no scale will take effect.

```javascript
getOnlyArea() : boolean;
```


### setOnlyArea(boolean) {#setOnlyArea-boolean-}

If this property is true , one Area will be output, and no scale will take effect.

```javascript
setOnlyArea(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTransparent() {#getTransparent--}

Indicates if the background of generated image should be transparent.

```javascript
getTransparent() : boolean;
```


**Remarks**

The default value is false. That means the background of the generated images is white.

### setTransparent(boolean) {#setTransparent-boolean-}

Indicates if the background of generated image should be transparent.

```javascript
setTransparent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false. That means the background of the generated images is white.

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](./iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](./iwarningcallback/)

### getPageSavingCallback() {#getPageSavingCallback--}

Control/Indicate progress of page saving process.

```javascript
getPageSavingCallback() : IPageSavingCallback;
```


**Returns**

[IPageSavingCallback](./ipagesavingcallback/)

### setPageSavingCallback(IPageSavingCallback) {#setPageSavingCallback-ipagesavingcallback-}

Control/Indicate progress of page saving process.

```javascript
setPageSavingCallback(value: IPageSavingCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](./ipagesavingcallback/) | The value to set. |

### setIsFontSubstitutionCharGranularity(boolean) {#setIsFontSubstitutionCharGranularity-boolean-}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
setIsFontSubstitutionCharGranularity(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
isFontSubstitutionCharGranularity() : boolean;
```


**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### setPageIndex(number) {#setPageIndex-number-}

Gets or sets the 0-based index of the first page to save.

```javascript
setPageIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Default is 0.

### getPageIndex() {#getPageIndex--}

Gets or sets the 0-based index of the first page to save.

```javascript
getPageIndex() : number;
```


**Remarks**

Default is 0.

### setPageCount(number) {#setPageCount-number-}

Gets or sets the number of pages to save.

```javascript
setPageCount(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered.

### getPageCount() {#getPageCount--}

Gets or sets the number of pages to save.

```javascript
getPageCount() : number;
```


**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered.

### isOptimized() {#isOptimized--}

Indicates whether to optimize the output elements.

```javascript
isOptimized() : boolean;
```


**Remarks**

Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

### setIsOptimized(boolean) {#setIsOptimized-boolean-}

Indicates whether to optimize the output elements.

```javascript
setIsOptimized(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

### getDefaultFont() {#getDefaultFont--}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
getDefaultFont() : string;
```


### setDefaultFont(string) {#setDefaultFont-string-}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
setDefaultFont(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
getCheckWorkbookDefaultFont() : boolean;
```


**Remarks**

Default is true.

### setCheckWorkbookDefaultFont(boolean) {#setCheckWorkbookDefaultFont-boolean-}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
setCheckWorkbookDefaultFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default is true.

### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}

Indicates whether to output a blank page when there is nothing to print.

```javascript
getOutputBlankPageWhenNothingToPrint() : boolean;
```


**Remarks**

Default is false.

### setOutputBlankPageWhenNothingToPrint(boolean) {#setOutputBlankPageWhenNothingToPrint-boolean-}

Indicates whether to output a blank page when there is nothing to print.

```javascript
setOutputBlankPageWhenNothingToPrint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default is false.

### getGridlineType() {#getGridlineType--}

Gets or sets gridline type.

```javascript
getGridlineType() : GridlineType;
```


**Returns**

[GridlineType](./gridlinetype/)

**Remarks**

Default is Dotted type.

### setGridlineType(GridlineType) {#setGridlineType-gridlinetype-}

Gets or sets gridline type.

```javascript
setGridlineType(value: GridlineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridlineType](./gridlinetype/) | The value to set. |

**Remarks**

Default is Dotted type.

### getTextCrossType() {#getTextCrossType--}

Gets or sets displaying text type when the text width is larger than cell width.

```javascript
getTextCrossType() : TextCrossType;
```


**Returns**

[TextCrossType](./textcrosstype/)

### setTextCrossType(TextCrossType) {#setTextCrossType-textcrosstype-}

Gets or sets displaying text type when the text width is larger than cell width.

```javascript
setTextCrossType(value: TextCrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCrossType](./textcrosstype/) | The value to set. |

### getDefaultEditLanguage() {#getDefaultEditLanguage--}

Gets or sets default edit language.

```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```


**Returns**

[DefaultEditLanguage](./defaulteditlanguage/)

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](./aspose.cells.defaulteditlanguage.auto/).

### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}

Gets or sets default edit language.

```javascript
setDefaultEditLanguage(value: DefaultEditLanguage) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DefaultEditLanguage](./defaulteditlanguage/) | The value to set. |

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](./aspose.cells.defaulteditlanguage.auto/).

### getSheetSet() {#getSheetSet--}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](./aspose.cells.rendering.sheetset.visible/).

```javascript
getSheetSet() : SheetSet;
```


**Returns**

[SheetSet](./sheetset/)

**Remarks**

The set is ignored when it is used in [SheetRender](./sheetrender/)

### setSheetSet(SheetSet) {#setSheetSet-sheetset-}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](./aspose.cells.rendering.sheetset.visible/).

```javascript
setSheetSet(value: SheetSet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](./sheetset/) | The value to set. |

**Remarks**

The set is ignored when it is used in [SheetRender](./sheetrender/)

### getEmfRenderSetting() {#getEmfRenderSetting--}

Setting for rendering Emf metafile.

```javascript
getEmfRenderSetting() : EmfRenderSetting;
```


**Returns**

[EmfRenderSetting](./emfrendersetting/)

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](./aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](./aspose.cells.emfrendersetting.emfonly/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### setEmfRenderSetting(EmfRenderSetting) {#setEmfRenderSetting-emfrendersetting-}

Setting for rendering Emf metafile.

```javascript
setEmfRenderSetting(value: EmfRenderSetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EmfRenderSetting](./emfrendersetting/) | The value to set. |

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](./aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](./aspose.cells.emfrendersetting.emfonly/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### setDesiredSize(number, number, boolean) {#setDesiredSize-number-number-boolean-}

Sets desired width and height of image.

```javascript
setDesiredSize(desiredWidth: number, desiredHeight: number, keepAspectRatio: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | number | desired width in pixels |
| desiredHeight | number | desired height in pixels |
| keepAspectRatio | boolean | whether to keep aspect ratio of origin image |


