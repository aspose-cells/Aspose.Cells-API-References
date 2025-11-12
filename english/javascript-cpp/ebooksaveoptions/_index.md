---
title: EbookSaveOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the options for saving ebook file.
type: docs
url: /javascript-cpp/ebooksaveoptions/
---

## EbookSaveOptions class

Represents the options for saving ebook file.

```javascript
class EbookSaveOptions extends HtmlSaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving ebook file. |
| [constructor(HtmlSaveOptions)](#constructor-htmlsaveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates options for saving ebook file. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [saveFormat](#saveFormat--)| SaveFormat | Readonly. Gets the save file format. |
| [clearData](#clearData--)| boolean | Make the workbook empty after saving the file. |
| [cachedFileFolder](#cachedFileFolder--)| string | The folder for temporary files that may be used as data cache. |
| [validateMergedAreas](#validateMergedAreas--)| boolean | Indicates whether validate merged cells before saving the file. |
| [mergeAreas](#mergeAreas--)| boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [createDirectory](#createDirectory--)| boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sortNames](#sortNames--)| boolean | Indicates whether sorting defined names before saving file. |
| [sortExternalNames](#sortExternalNames--)| boolean | Indicates whether sorting external defined names before saving file. |
| [refreshChartCache](#refreshChartCache--)| boolean | Indicates whether refreshing chart cache data |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [checkExcelRestriction](#checkExcelRestriction--)| boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [updateSmartArt](#updateSmartArt--)| boolean | Indicates whether updating smart art setting. The default value is false. |
| [encryptDocumentProperties](#encryptDocumentProperties--)| boolean | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [ignoreInvisibleShapes](#ignoreInvisibleShapes--)| boolean | Indicate whether exporting those not visible shapes |
| [pageTitle](#pageTitle--)| string | The title of the html page. Only for saving to html stream. |
| [attachedFilesDirectory](#attachedFilesDirectory--)| string | The directory that the attached files will be saved to. Only for saving to html stream. |
| [attachedFilesUrlPrefix](#attachedFilesUrlPrefix--)| string | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [defaultFontName](#defaultFontName--)| string | Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [addGenericFont](#addGenericFont--)| boolean | Indicates whether to add a generic font to CSS font-family. The default value is true |
| [worksheetScalable](#worksheetScalable--)| boolean | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [isExportComments](#isExportComments--)| boolean | Indicates if exporting comments when saving file to html, the default value is false. |
| [exportCommentsType](#exportCommentsType--)| PrintCommentsType | Represents type of exporting comments to html files. |
| [disableDownlevelRevealedComments](#disableDownlevelRevealedComments--)| boolean | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [isExpImageToTempDir](#isExpImageToTempDir--)| boolean | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [imageScalable](#imageScalable--)| boolean | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [widthScalable](#widthScalable--)| boolean | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [exportSingleTab](#exportSingleTab--)| boolean | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [exportImagesAsBase64](#exportImagesAsBase64--)| boolean | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [exportActiveWorksheetOnly](#exportActiveWorksheetOnly--)| boolean | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [exportPrintAreaOnly](#exportPrintAreaOnly--)| boolean | Indicates if only exporting the print area to html file. The default value is false. |
| [exportArea](#exportArea--)| CellArea | Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [parseHtmlTagInCell](#parseHtmlTagInCell--)| boolean | Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [htmlCrossStringType](#htmlCrossStringType--)| HtmlCrossType | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [hiddenColDisplayType](#hiddenColDisplayType--)| HtmlHiddenColDisplayType | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [hiddenRowDisplayType](#hiddenRowDisplayType--)| HtmlHiddenRowDisplayType | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [encoding](#encoding--)| EncodingType | If not set,use Encoding.UTF8 as default enconding type. |
| [filePathProvider](#filePathProvider--)| IFilePathProvider | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [imageOptions](#imageOptions--)| ImageOrPrintOptions | Readonly. Get the ImageOrPrintOptions object before exporting |
| [saveAsSingleFile](#saveAsSingleFile--)| boolean | Indicates whether save the html as single file. The default value is false. |
| [showAllSheets](#showAllSheets--)| boolean | Indicates whether showing all sheets when saving  as a single html file. |
| [exportPageHeaders](#exportPageHeaders--)| boolean | Indicates whether exporting page headers. |
| [exportPageFooters](#exportPageFooters--)| boolean | Indicates whether exporting page headers. |
| [exportHiddenWorksheet](#exportHiddenWorksheet--)| boolean | Indicating if exporting the hidden worksheet content.The default value is true. |
| [presentationPreference](#presentationPreference--)| boolean | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [cellCssPrefix](#cellCssPrefix--)| string | Gets and sets the prefix of the css name,the default value is "". |
| [tableCssId](#tableCssId--)| string | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [isFullPathLink](#isFullPathLink--)| boolean | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [exportWorksheetCSSSeparately](#exportWorksheetCSSSeparately--)| boolean | Indicating whether export the worksheet css separately.The default value is false. |
| [exportSimilarBorderStyle](#exportSimilarBorderStyle--)| boolean | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [mergeEmptyTdForcely](#mergeEmptyTdForcely--)| boolean | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [mergeEmptyTdType](#mergeEmptyTdType--)| MergeEmptyTdType | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [exportCellCoordinate](#exportCellCoordinate--)| boolean | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [exportExtraHeadings](#exportExtraHeadings--)| boolean | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [exportRowColumnHeadings](#exportRowColumnHeadings--)| boolean | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [exportFormula](#exportFormula--)| boolean | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [addTooltipText](#addTooltipText--)| boolean | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [exportGridLines](#exportGridLines--)| boolean | Indicating whether exporting the gridlines.The default value is false. |
| [exportBogusRowData](#exportBogusRowData--)| boolean | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [excludeUnusedStyles](#excludeUnusedStyles--)| boolean | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [exportDocumentProperties](#exportDocumentProperties--)| boolean | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [exportWorksheetProperties](#exportWorksheetProperties--)| boolean | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [exportWorkbookProperties](#exportWorkbookProperties--)| boolean | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [exportFrameScriptsAndProperties](#exportFrameScriptsAndProperties--)| boolean | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [exportDataOptions](#exportDataOptions--)| HtmlExportDataOptions | Indicating the rule of exporting html file data.The default value is All. |
| [linkTargetType](#linkTargetType--)| HtmlLinkTargetType | Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
| [isIECompatible](#isIECompatible--)| boolean | Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [formatDataIgnoreColumnWidth](#formatDataIgnoreColumnWidth--)| boolean | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [calculateFormula](#calculateFormula--)| boolean | Indicates whether to calculate formulas before saving html file. |
| [isJsBrowserCompatible](#isJsBrowserCompatible--)| boolean | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [isMobileCompatible](#isMobileCompatible--)| boolean | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [cssStyles](#cssStyles--)| string | Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example> |
| [hideOverflowWrappedText](#hideOverflowWrappedText--)| boolean | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [isBorderCollapsed](#isBorderCollapsed--)| boolean | Indicates whether the table borders are collapsed. The default value is true. |
| [encodeEntityAsCode](#encodeEntityAsCode--)| boolean | Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [officeMathOutputMode](#officeMathOutputMode--)| HtmlOfficeMathOutputType | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [cellNameAttribute](#cellNameAttribute--)| string | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [disableCss](#disableCss--)| boolean | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [enableCssCustomProperties](#enableCssCustomProperties--)| boolean | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [htmlVersion](#htmlVersion--)| HtmlVersion | Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default. |
| [sheetSet](#sheetSet--)| SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [layoutMode](#layoutMode--)| HtmlLayoutMode | Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/) |
| [embeddedFontType](#embeddedFontType--)| HtmlEmbeddedFontType | Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html. |


### constructor() {#constructor--}

Creates options for saving ebook file.

```javascript
constructor();
```


### constructor(HtmlSaveOptions) {#constructor-htmlsaveoptions-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: HtmlSaveOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | HtmlSaveOptions | The parent object. |

### constructor(SaveFormat) {#constructor-saveformat-}

Creates options for saving ebook file.

```javascript
constructor(saveFormat: SaveFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be [SaveFormat.Epub](../saveformat.epub/) or [SaveFormat.Azw3](../saveformat.azw3/). |

### saveFormat {#saveFormat--}

Readonly. Gets the save file format.

```javascript
saveFormat : SaveFormat;
```


### clearData {#clearData--}

Make the workbook empty after saving the file.

```javascript
clearData : boolean;
```


### cachedFileFolder {#cachedFileFolder--}

The folder for temporary files that may be used as data cache.

```javascript
cachedFileFolder : string;
```


**Remarks**

If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.

### validateMergedAreas {#validateMergedAreas--}

Indicates whether validate merged cells before saving the file.

```javascript
validateMergedAreas : boolean;
```


**Remarks**

The default value is false.

### mergeAreas {#mergeAreas--}

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
mergeAreas : boolean;
```


**Remarks**

The default value is false.

### createDirectory {#createDirectory--}

If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
createDirectory : boolean;
```


**Remarks**

The default value is false.

### sortNames {#sortNames--}

Indicates whether sorting defined names before saving file.

```javascript
sortNames : boolean;
```


### sortExternalNames {#sortExternalNames--}

Indicates whether sorting external defined names before saving file.

```javascript
sortExternalNames : boolean;
```


### refreshChartCache {#refreshChartCache--}

Indicates whether refreshing chart cache data

```javascript
refreshChartCache : boolean;
```


### warningCallback {#warningCallback--}

Gets or sets warning callback.

```javascript
warningCallback : IWarningCallback;
```


### checkExcelRestriction {#checkExcelRestriction--}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
checkExcelRestriction : boolean;
```


### updateSmartArt {#updateSmartArt--}

Indicates whether updating smart art setting. The default value is false.

```javascript
updateSmartArt : boolean;
```


**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### encryptDocumentProperties {#encryptDocumentProperties--}

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
encryptDocumentProperties : boolean;
```


**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

### ignoreInvisibleShapes {#ignoreInvisibleShapes--}

Indicate whether exporting those not visible shapes

```javascript
ignoreInvisibleShapes : boolean;
```


**Remarks**

The default values is false.

### pageTitle {#pageTitle--}

The title of the html page. Only for saving to html stream.

```javascript
pageTitle : string;
```


### attachedFilesDirectory {#attachedFilesDirectory--}

The directory that the attached files will be saved to. Only for saving to html stream.

```javascript
attachedFilesDirectory : string;
```


### attachedFilesUrlPrefix {#attachedFilesUrlPrefix--}

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

```javascript
attachedFilesUrlPrefix : string;
```


### defaultFontName {#defaultFontName--}

Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```javascript
defaultFontName : string;
```


### addGenericFont {#addGenericFont--}

Indicates whether to add a generic font to CSS font-family. The default value is true

```javascript
addGenericFont : boolean;
```


### worksheetScalable {#worksheetScalable--}

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```javascript
worksheetScalable : boolean;
```


### isExportComments {#isExportComments--}

Indicates if exporting comments when saving file to html, the default value is false.

```javascript
isExportComments : boolean;
```


### exportCommentsType {#exportCommentsType--}

Represents type of exporting comments to html files.

```javascript
exportCommentsType : PrintCommentsType;
```


### disableDownlevelRevealedComments {#disableDownlevelRevealedComments--}

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

```javascript
disableDownlevelRevealedComments : boolean;
```


### isExpImageToTempDir {#isExpImageToTempDir--}

Indicates whether exporting image files to temp directory. Only for saving to html stream.

```javascript
isExpImageToTempDir : boolean;
```


### imageScalable {#imageScalable--}

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

```javascript
imageScalable : boolean;
```


### widthScalable {#widthScalable--}

Indicates whether exporting column width in unit of scale to html. The default value is false.

```javascript
widthScalable : boolean;
```


### exportSingleTab {#exportSingleTab--}

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```javascript
exportSingleTab : boolean;
```


### exportImagesAsBase64 {#exportImagesAsBase64--}

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.

```javascript
exportImagesAsBase64 : boolean;
```


**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### exportActiveWorksheetOnly {#exportActiveWorksheetOnly--}

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```javascript
exportActiveWorksheetOnly : boolean;
```


### exportPrintAreaOnly {#exportPrintAreaOnly--}

Indicates if only exporting the print area to html file. The default value is false.

```javascript
exportPrintAreaOnly : boolean;
```


### exportArea {#exportArea--}

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```javascript
exportArea : CellArea;
```


### parseHtmlTagInCell {#parseHtmlTagInCell--}

Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true.

```javascript
parseHtmlTagInCell : boolean;
```


### htmlCrossStringType {#htmlCrossStringType--}

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```javascript
htmlCrossStringType : HtmlCrossType;
```


### hiddenColDisplayType {#hiddenColDisplayType--}

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

```javascript
hiddenColDisplayType : HtmlHiddenColDisplayType;
```


### hiddenRowDisplayType {#hiddenRowDisplayType--}

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```javascript
hiddenRowDisplayType : HtmlHiddenRowDisplayType;
```


### encoding {#encoding--}

If not set,use Encoding.UTF8 as default enconding type.

```javascript
encoding : EncodingType;
```


### filePathProvider {#filePathProvider--}

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

```javascript
filePathProvider : IFilePathProvider;
```


### imageOptions {#imageOptions--}

Readonly. Get the ImageOrPrintOptions object before exporting

```javascript
imageOptions : ImageOrPrintOptions;
```


### saveAsSingleFile {#saveAsSingleFile--}

Indicates whether save the html as single file. The default value is false.

```javascript
saveAsSingleFile : boolean;
```


**Remarks**

If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### showAllSheets {#showAllSheets--}

Indicates whether showing all sheets when saving  as a single html file.

```javascript
showAllSheets : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### exportPageHeaders {#exportPageHeaders--}

Indicates whether exporting page headers.

```javascript
exportPageHeaders : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### exportPageFooters {#exportPageFooters--}

Indicates whether exporting page headers.

```javascript
exportPageFooters : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### exportHiddenWorksheet {#exportHiddenWorksheet--}

Indicating if exporting the hidden worksheet content.The default value is true.

```javascript
exportHiddenWorksheet : boolean;
```


### presentationPreference {#presentationPreference--}

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```javascript
presentationPreference : boolean;
```


### cellCssPrefix {#cellCssPrefix--}

Gets and sets the prefix of the css name,the default value is "".

```javascript
cellCssPrefix : string;
```


### tableCssId {#tableCssId--}

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```javascript
tableCssId : string;
```


### isFullPathLink {#isFullPathLink--}

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

```javascript
isFullPathLink : boolean;
```


### exportWorksheetCSSSeparately {#exportWorksheetCSSSeparately--}

Indicating whether export the worksheet css separately.The default value is false.

```javascript
exportWorksheetCSSSeparately : boolean;
```


### exportSimilarBorderStyle {#exportSimilarBorderStyle--}

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```javascript
exportSimilarBorderStyle : boolean;
```


### mergeEmptyTdForcely {#mergeEmptyTdForcely--}

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

```javascript
mergeEmptyTdForcely : boolean;
```


### mergeEmptyTdType {#mergeEmptyTdType--}

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.

```javascript
mergeEmptyTdType : MergeEmptyTdType;
```


### exportCellCoordinate {#exportCellCoordinate--}

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

```javascript
exportCellCoordinate : boolean;
```


### exportExtraHeadings {#exportExtraHeadings--}

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```javascript
exportExtraHeadings : boolean;
```


### exportRowColumnHeadings {#exportRowColumnHeadings--}

Indicates whether exports sheet's row and column headings when saving to HTML files.

```javascript
exportRowColumnHeadings : boolean;
```


**Remarks**

The default value is false.

### exportFormula {#exportFormula--}

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```javascript
exportFormula : boolean;
```


### addTooltipText {#addTooltipText--}

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

```javascript
addTooltipText : boolean;
```


### exportGridLines {#exportGridLines--}

Indicating whether exporting the gridlines.The default value is false.

```javascript
exportGridLines : boolean;
```


### exportBogusRowData {#exportBogusRowData--}

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
exportBogusRowData : boolean;
```


### excludeUnusedStyles {#excludeUnusedStyles--}

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

```javascript
excludeUnusedStyles : boolean;
```


### exportDocumentProperties {#exportDocumentProperties--}

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
exportDocumentProperties : boolean;
```


### exportWorksheetProperties {#exportWorksheetProperties--}

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
exportWorksheetProperties : boolean;
```


### exportWorkbookProperties {#exportWorkbookProperties--}

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
exportWorkbookProperties : boolean;
```


### exportFrameScriptsAndProperties {#exportFrameScriptsAndProperties--}

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
exportFrameScriptsAndProperties : boolean;
```


### exportDataOptions {#exportDataOptions--}

Indicating the rule of exporting html file data.The default value is All.

```javascript
exportDataOptions : HtmlExportDataOptions;
```


### linkTargetType {#linkTargetType--}

Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent.

```javascript
linkTargetType : HtmlLinkTargetType;
```


### isIECompatible {#isIECompatible--}

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

```javascript
isIECompatible : boolean;
```


### formatDataIgnoreColumnWidth {#formatDataIgnoreColumnWidth--}

Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

```javascript
formatDataIgnoreColumnWidth : boolean;
```


### calculateFormula {#calculateFormula--}

Indicates whether to calculate formulas before saving html file.

```javascript
calculateFormula : boolean;
```


**Remarks**

The default value is false.

### isJsBrowserCompatible {#isJsBrowserCompatible--}

Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

```javascript
isJsBrowserCompatible : boolean;
```


### isMobileCompatible {#isMobileCompatible--}

Indicates whether the output HTML is compatible with mobile devices. The default value is false.

```javascript
isMobileCompatible : boolean;
```


### cssStyles {#cssStyles--}

Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example>

```javascript
cssStyles : string;
```


### hideOverflowWrappedText {#hideOverflowWrappedText--}

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

```javascript
hideOverflowWrappedText : boolean;
```


### isBorderCollapsed {#isBorderCollapsed--}

Indicates whether the table borders are collapsed. The default value is true.

```javascript
isBorderCollapsed : boolean;
```


### encodeEntityAsCode {#encodeEntityAsCode--}

Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false.

```javascript
encodeEntityAsCode : boolean;
```


### officeMathOutputMode {#officeMathOutputMode--}

Indicates how export OfficeMath objects to HTML, Default value is Image.

```javascript
officeMathOutputMode : HtmlOfficeMathOutputType;
```


### cellNameAttribute {#cellNameAttribute--}

Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```javascript
cellNameAttribute : string;
```


### disableCss {#disableCss--}

Indicates whether only inline styles are applied, without relying on CSS. The default value is false.

```javascript
disableCss : boolean;
```


### enableCssCustomProperties {#enableCssCustomProperties--}

Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false.

```javascript
enableCssCustomProperties : boolean;
```


### htmlVersion {#htmlVersion--}

Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default.

```javascript
htmlVersion : HtmlVersion;
```


### sheetSet {#sheetSet--}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
sheetSet : SheetSet;
```


### layoutMode {#layoutMode--}

Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/)

```javascript
layoutMode : HtmlLayoutMode;
```


### embeddedFontType {#embeddedFontType--}

Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html.

```javascript
embeddedFontType : HtmlEmbeddedFontType;
```



