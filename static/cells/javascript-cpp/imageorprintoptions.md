##ImageOrPrintOptions
Allows to specify options when rendering worksheet to images printing worksheet or rendering chart to image.
## ImageOrPrintOptions class
Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.
```javascript
class ImageOrPrintOptions;
```
### Example
```javascript
const { Workbook, ImageOrPrintOptions } = AsposeCells;
//Set Image Or Print Options
var options = new ImageOrPrintOptions();
//set Horizontal resolution
options.horizontalResolution = 200;
//set Vertica; Resolution
options.verticalResolution = 300;
//Instantiate Workbook
var book = new Workbook(data);
//Save chart as Image using ImageOrPrint Options
var uint8Array = book.worksheets.get(0).charts.get(0).toImage(options);
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Ctor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [printWithStatusDialog](#printWithStatusDialog--)| boolean | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [horizontalResolution](#horizontalResolution--)| number | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [verticalResolution](#verticalResolution--)| number | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [tiffCompression](#tiffCompression--)| TiffCompression | Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
| [tiffColorDepth](#tiffColorDepth--)| ColorDepth | Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
| [tiffBinarizationMethod](#tiffBinarizationMethod--)| ImageBinarizationMethod | Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [printingPage](#printingPage--)| PrintingPageType | Indicates which pages will not be printed. |
| [quality](#quality--)| number | Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
| [onePagePerSheet](#onePagePerSheet--)| boolean | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [allColumnsInOnePagePerSheet](#allColumnsInOnePagePerSheet--)| boolean | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [drawObjectEventHandler](#drawObjectEventHandler--)| DrawObjectEventHandler | Implements this interface to get DrawObject and Bound when rendering. |
| [embededImageNameInSvg](#embededImageNameInSvg--)| string | Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [sVGFitToViewPort](#sVGFitToViewPort--)| boolean | if this property is true, the generated svg will fit to view port. |
| [svgCssPrefix](#svgCssPrefix--)| string | Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [onlyArea](#onlyArea--)| boolean | If this property is true , one Area will be output, and no scale will take effect. |
| [transparent](#transparent--)| boolean | Indicates if the background of generated image should be transparent. |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [pageSavingCallback](#pageSavingCallback--)| IPageSavingCallback | Control/Indicate progress of page saving process. |
| [isFontSubstitutionCharGranularity](#isFontSubstitutionCharGranularity--)| boolean | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [pageIndex](#pageIndex--)| number | Gets or sets the 0-based index of the first page to save. |
| [pageCount](#pageCount--)| number | Gets or sets the number of pages to save. |
| [isOptimized](#isOptimized--)| boolean | Indicates whether to optimize the output elements. |
| [defaultFont](#defaultFont--)| string | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [checkWorkbookDefaultFont](#checkWorkbookDefaultFont--)| boolean | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [outputBlankPageWhenNothingToPrint](#outputBlankPageWhenNothingToPrint--)| boolean | Indicates whether to output a blank page when there is nothing to print. |
| [gridlineType](#gridlineType--)| GridlineType | Gets or sets gridline type. |
| [gridlineColor](#gridlineColor--)| Color | Gets or sets gridline colr. |
| [textCrossType](#textCrossType--)| TextCrossType | Gets or sets displaying text type when the text width is larger than cell width. |
| [defaultEditLanguage](#defaultEditLanguage--)| DefaultEditLanguage | Gets or sets default edit language. |
| [sheetSet](#sheetSet--)| SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [emfRenderSetting](#emfRenderSetting--)| EmfRenderSetting | Setting for rendering Emf metafiles in source file. |
| [customRenderSettings](#customRenderSettings--)| CustomRenderSettings | Gets or sets custom settings during rendering. |
## Methods
| Method | Description |
| --- | --- |
| [setDesiredSize(number, number, boolean)](#setDesiredSize-number-number-boolean-)| Sets desired width and height of image. |
| [getImageType()](#getImageType--)| Gets or sets the format of the generated images. default value: PNG. |
| [setImageType(ImageType)](#setImageType-imagetype-)| Gets or sets the format of the generated images. default value: PNG. |
### constructor() {#constructor--}
Ctor.
```javascript
constructor();
```
### printWithStatusDialog {#printWithStatusDialog--}
If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.
```javascript
printWithStatusDialog : boolean;
```
### horizontalResolution {#horizontalResolution--}
Gets or sets the horizontal resolution for generated images, in dots per inch.
```javascript
horizontalResolution : number;
```
**Remarks**
ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para
### verticalResolution {#verticalResolution--}
Gets or sets the vertical resolution for generated images, in dots per inch.
```javascript
verticalResolution : number;
```
**Remarks**
ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para
### tiffCompression {#tiffCompression--}
Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format.
```javascript
tiffCompression : TiffCompression;
```
**Remarks**
Has effect only when saving to TIFF. The default value is Lzw.
### tiffColorDepth {#tiffColorDepth--}
Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format.
```javascript
tiffColorDepth : ColorDepth;
```
**Remarks**
Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.
### tiffBinarizationMethod {#tiffBinarizationMethod--}
Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4.
```javascript
tiffBinarizationMethod : ImageBinarizationMethod;
```
**Remarks**
The default value is FloydSteinbergDithering.
### printingPage {#printingPage--}
Indicates which pages will not be printed.
```javascript
printingPage : PrintingPageType;
```
### quality {#quality--}
Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100
```javascript
quality : number;
```
**Remarks**
Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.
### onePagePerSheet {#onePagePerSheet--}
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
```javascript
onePagePerSheet : boolean;
```
### allColumnsInOnePagePerSheet {#allColumnsInOnePagePerSheet--}
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
```javascript
allColumnsInOnePagePerSheet : boolean;
```
### drawObjectEventHandler {#drawObjectEventHandler--}
Implements this interface to get DrawObject and Bound when rendering.
```javascript
drawObjectEventHandler : DrawObjectEventHandler;
```
### embededImageNameInSvg {#embededImageNameInSvg--}
Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"
```javascript
embededImageNameInSvg : string;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
### sVGFitToViewPort {#sVGFitToViewPort--}
if this property is true, the generated svg will fit to view port.
```javascript
sVGFitToViewPort : boolean;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.FitToViewPort](../svgimageoptions.fittoviewport/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
### svgCssPrefix {#svgCssPrefix--}
Gets and sets the prefix of the css name in svg,the default value is empty string.
```javascript
svgCssPrefix : string;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.CssPrefix](../svgimageoptions.cssprefix/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
### onlyArea {#onlyArea--}
If this property is true , one Area will be output, and no scale will take effect.
```javascript
onlyArea : boolean;
```
### transparent {#transparent--}
Indicates if the background of generated image should be transparent.
```javascript
transparent : boolean;
```
**Remarks**
The default value is false. That means the background of the generated images is white.
### warningCallback {#warningCallback--}
Gets or sets warning callback.
```javascript
warningCallback : IWarningCallback;
```
### pageSavingCallback {#pageSavingCallback--}
Control/Indicate progress of page saving process.
```javascript
pageSavingCallback : IPageSavingCallback;
```
### isFontSubstitutionCharGranularity {#isFontSubstitutionCharGranularity--}
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
```javascript
isFontSubstitutionCharGranularity : boolean;
```
**Remarks**
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
### pageIndex {#pageIndex--}
Gets or sets the 0-based index of the first page to save.
```javascript
pageIndex : number;
```
**Remarks**
Default is 0.
### pageCount {#pageCount--}
Gets or sets the number of pages to save.
```javascript
pageCount : number;
```
**Remarks**
Default is System.Int32.MaxValue which means all pages will be rendered.
### isOptimized {#isOptimized--}
Indicates whether to optimize the output elements.
```javascript
isOptimized : boolean;
```
**Remarks**
Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.
### defaultFont {#defaultFont--}
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.
```javascript
defaultFont : string;
```
### checkWorkbookDefaultFont {#checkWorkbookDefaultFont--}
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.
```javascript
checkWorkbookDefaultFont : boolean;
```
**Remarks**
Default is true.
### outputBlankPageWhenNothingToPrint {#outputBlankPageWhenNothingToPrint--}
Indicates whether to output a blank page when there is nothing to print.
```javascript
outputBlankPageWhenNothingToPrint : boolean;
```
**Remarks**
Default is false.
### gridlineType {#gridlineType--}
Gets or sets gridline type.
```javascript
gridlineType : GridlineType;
```
**Remarks**
Default is Dotted type.
### gridlineColor {#gridlineColor--}
Gets or sets gridline colr.
```javascript
gridlineColor : Color;
```
**Remarks**
It will ignore the gridline color settings in the source file.
### textCrossType {#textCrossType--}
Gets or sets displaying text type when the text width is larger than cell width.
```javascript
textCrossType : TextCrossType;
```
### defaultEditLanguage {#defaultEditLanguage--}
Gets or sets default edit language.
```javascript
defaultEditLanguage : DefaultEditLanguage;
```
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).
### sheetSet {#sheetSet--}
Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).
```javascript
sheetSet : SheetSet;
```
**Remarks**
The set is ignored when it is used in [SheetRender](../sheetrender/)
### emfRenderSetting {#emfRenderSetting--}
Setting for rendering Emf metafiles in source file.
```javascript
emfRenderSetting : EmfRenderSetting;
```
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
### customRenderSettings {#customRenderSettings--}
Gets or sets custom settings during rendering.
```javascript
customRenderSettings : CustomRenderSettings;
```
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
**Remarks**
ara>The width and height of the output image in pixels will be only based on the set desired width and height.</para> <para>The [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) will not effect the width and height of the output image in this case.</para
### getImageType() {#getImageType--}
Gets or sets the format of the generated images. default value: PNG.
```javascript
getImageType() : ImageType;
```
**Returns**
[ImageType](../imagetype/)
### setImageType(ImageType) {#setImageType-imagetype-}
Gets or sets the format of the generated images. default value: PNG.
```javascript
setImageType(value: ImageType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageType](../imagetype/) | The value to set. |
