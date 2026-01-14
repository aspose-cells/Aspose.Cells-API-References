---
title: HtmlSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options for saving html file.
type: docs
url: /nodejs-cpp/htmlsaveoptions/
---

## HtmlSaveOptions class

Represents the options for saving html file.

```javascript
class HtmlSaveOptions extends SaveOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving html file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates options for saving htm file. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
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
| [officeMathOutputMode](#officeMathOutputMode--)| HtmlOfficeMathOutputType | Indicates how OfficeMath objects are exported to HTML, Default value is Image. |
| [cellNameAttribute](#cellNameAttribute--)| string | Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [disableCss](#disableCss--)| boolean | Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [enableCssCustomProperties](#enableCssCustomProperties--)| boolean | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [htmlVersion](#htmlVersion--)| HtmlVersion | Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default. |
| [sheetSet](#sheetSet--)| SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [layoutMode](#layoutMode--)| HtmlLayoutMode | Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/) |
| [embeddedFontType](#embeddedFontType--)| HtmlEmbeddedFontType | Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html. |
| [exportNamedRangeAnchors](#exportNamedRangeAnchors--)| boolean | Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true. |
| [dataBarRenderMode](#dataBarRenderMode--)| DataBarRenderMode | Represents the mode of how to render DataBar when converting Excel files to html files. Default value is [DataBarRenderMode.BackgroundColor](../databarrendermode.backgroundcolor/). |
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

## Methods

| Method | Description |
| --- | --- |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--)| <b>@deprecated.</b> Please use the 'ignoreInvisibleShapes' property instead. Indicate whether exporting those not visible shapes |
| [setIgnoreInvisibleShapes(boolean)](#setIgnoreInvisibleShapes-boolean-)| <b>@deprecated.</b> Please use the 'ignoreInvisibleShapes' property instead. Indicate whether exporting those not visible shapes |
| [getPageTitle()](#getPageTitle--)| <b>@deprecated.</b> Please use the 'pageTitle' property instead. The title of the html page. Only for saving to html stream. |
| [setPageTitle(string)](#setPageTitle-string-)| <b>@deprecated.</b> Please use the 'pageTitle' property instead. The title of the html page. Only for saving to html stream. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--)| <b>@deprecated.</b> Please use the 'attachedFilesDirectory' property instead. The directory that the attached files will be saved to. Only for saving to html stream. |
| [setAttachedFilesDirectory(string)](#setAttachedFilesDirectory-string-)| <b>@deprecated.</b> Please use the 'attachedFilesDirectory' property instead. The directory that the attached files will be saved to. Only for saving to html stream. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--)| <b>@deprecated.</b> Please use the 'attachedFilesUrlPrefix' property instead. Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [setAttachedFilesUrlPrefix(string)](#setAttachedFilesUrlPrefix-string-)| <b>@deprecated.</b> Please use the 'attachedFilesUrlPrefix' property instead. Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [getDefaultFontName()](#getDefaultFontName--)| <b>@deprecated.</b> Please use the 'defaultFontName' property instead. Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [setDefaultFontName(string)](#setDefaultFontName-string-)| <b>@deprecated.</b> Please use the 'defaultFontName' property instead. Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [getAddGenericFont()](#getAddGenericFont--)| <b>@deprecated.</b> Please use the 'addGenericFont' property instead. Indicates whether to add a generic font to CSS font-family. The default value is true |
| [setAddGenericFont(boolean)](#setAddGenericFont-boolean-)| <b>@deprecated.</b> Please use the 'addGenericFont' property instead. Indicates whether to add a generic font to CSS font-family. The default value is true |
| [getWorksheetScalable()](#getWorksheetScalable--)| <b>@deprecated.</b> Please use the 'worksheetScalable' property instead. Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [setWorksheetScalable(boolean)](#setWorksheetScalable-boolean-)| <b>@deprecated.</b> Please use the 'worksheetScalable' property instead. Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [isExportComments()](#isExportComments--)| <b>@deprecated.</b> Please use the 'isExportComments' property instead. Indicates if exporting comments when saving file to html, the default value is false. |
| [setIsExportComments(boolean)](#setIsExportComments-boolean-)| <b>@deprecated.</b> Please use the 'isExportComments' property instead. Indicates if exporting comments when saving file to html, the default value is false. |
| [getExportCommentsType()](#getExportCommentsType--)| <b>@deprecated.</b> Please use the 'exportCommentsType' property instead. Represents type of exporting comments to html files. |
| [setExportCommentsType(PrintCommentsType)](#setExportCommentsType-printcommentstype-)| <b>@deprecated.</b> Please use the 'exportCommentsType' property instead. Represents type of exporting comments to html files. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--)| <b>@deprecated.</b> Please use the 'disableDownlevelRevealedComments' property instead. Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [setDisableDownlevelRevealedComments(boolean)](#setDisableDownlevelRevealedComments-boolean-)| <b>@deprecated.</b> Please use the 'disableDownlevelRevealedComments' property instead. Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [isExpImageToTempDir()](#isExpImageToTempDir--)| <b>@deprecated.</b> Please use the 'isExpImageToTempDir' property instead. Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [setIsExpImageToTempDir(boolean)](#setIsExpImageToTempDir-boolean-)| <b>@deprecated.</b> Please use the 'isExpImageToTempDir' property instead. Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [getImageScalable()](#getImageScalable--)| <b>@deprecated.</b> Please use the 'imageScalable' property instead. Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [setImageScalable(boolean)](#setImageScalable-boolean-)| <b>@deprecated.</b> Please use the 'imageScalable' property instead. Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [getWidthScalable()](#getWidthScalable--)| <b>@deprecated.</b> Please use the 'widthScalable' property instead. Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [setWidthScalable(boolean)](#setWidthScalable-boolean-)| <b>@deprecated.</b> Please use the 'widthScalable' property instead. Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [getExportSingleTab()](#getExportSingleTab--)| <b>@deprecated.</b> Please use the 'exportSingleTab' property instead. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [setExportSingleTab(boolean)](#setExportSingleTab-boolean-)| <b>@deprecated.</b> Please use the 'exportSingleTab' property instead. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--)| <b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [setExportImagesAsBase64(boolean)](#setExportImagesAsBase64-boolean-)| <b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--)| <b>@deprecated.</b> Please use the 'exportActiveWorksheetOnly' property instead. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [setExportActiveWorksheetOnly(boolean)](#setExportActiveWorksheetOnly-boolean-)| <b>@deprecated.</b> Please use the 'exportActiveWorksheetOnly' property instead. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--)| <b>@deprecated.</b> Please use the 'exportPrintAreaOnly' property instead. Indicates if only exporting the print area to html file. The default value is false. |
| [setExportPrintAreaOnly(boolean)](#setExportPrintAreaOnly-boolean-)| <b>@deprecated.</b> Please use the 'exportPrintAreaOnly' property instead. Indicates if only exporting the print area to html file. The default value is false. |
| [getExportArea()](#getExportArea--)| <b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| <b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--)| <b>@deprecated.</b> Please use the 'parseHtmlTagInCell' property instead. Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [setParseHtmlTagInCell(boolean)](#setParseHtmlTagInCell-boolean-)| <b>@deprecated.</b> Please use the 'parseHtmlTagInCell' property instead. Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--)| <b>@deprecated.</b> Please use the 'htmlCrossStringType' property instead. Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [setHtmlCrossStringType(HtmlCrossType)](#setHtmlCrossStringType-htmlcrosstype-)| <b>@deprecated.</b> Please use the 'htmlCrossStringType' property instead. Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--)| <b>@deprecated.</b> Please use the 'hiddenColDisplayType' property instead. Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [setHiddenColDisplayType(HtmlHiddenColDisplayType)](#setHiddenColDisplayType-htmlhiddencoldisplaytype-)| <b>@deprecated.</b> Please use the 'hiddenColDisplayType' property instead. Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--)| <b>@deprecated.</b> Please use the 'hiddenRowDisplayType' property instead. Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [setHiddenRowDisplayType(HtmlHiddenRowDisplayType)](#setHiddenRowDisplayType-htmlhiddenrowdisplaytype-)| <b>@deprecated.</b> Please use the 'hiddenRowDisplayType' property instead. Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [getEncoding()](#getEncoding--)| <b>@deprecated.</b> Please use the 'encoding' property instead. If not set,use Encoding.UTF8 as default enconding type. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| <b>@deprecated.</b> Please use the 'encoding' property instead. If not set,use Encoding.UTF8 as default enconding type. |
| [getFilePathProvider()](#getFilePathProvider--)| <b>@deprecated.</b> Please use the 'filePathProvider' property instead. Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [setFilePathProvider(IFilePathProvider)](#setFilePathProvider-ifilepathprovider-)| <b>@deprecated.</b> Please use the 'filePathProvider' property instead. Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [getImageOptions()](#getImageOptions--)| <b>@deprecated.</b> Please use the 'imageOptions' property instead. Get the ImageOrPrintOptions object before exporting |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--)| <b>@deprecated.</b> Please use the 'saveAsSingleFile' property instead. Indicates whether save the html as single file. The default value is false. |
| [setSaveAsSingleFile(boolean)](#setSaveAsSingleFile-boolean-)| <b>@deprecated.</b> Please use the 'saveAsSingleFile' property instead. Indicates whether save the html as single file. The default value is false. |
| [getShowAllSheets()](#getShowAllSheets--)| <b>@deprecated.</b> Please use the 'showAllSheets' property instead. Indicates whether showing all sheets when saving  as a single html file. |
| [setShowAllSheets(boolean)](#setShowAllSheets-boolean-)| <b>@deprecated.</b> Please use the 'showAllSheets' property instead. Indicates whether showing all sheets when saving  as a single html file. |
| [getExportPageHeaders()](#getExportPageHeaders--)| <b>@deprecated.</b> Please use the 'exportPageHeaders' property instead. Indicates whether exporting page headers. |
| [setExportPageHeaders(boolean)](#setExportPageHeaders-boolean-)| <b>@deprecated.</b> Please use the 'exportPageHeaders' property instead. Indicates whether exporting page headers. |
| [getExportPageFooters()](#getExportPageFooters--)| <b>@deprecated.</b> Please use the 'exportPageFooters' property instead. Indicates whether exporting page headers. |
| [setExportPageFooters(boolean)](#setExportPageFooters-boolean-)| <b>@deprecated.</b> Please use the 'exportPageFooters' property instead. Indicates whether exporting page headers. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--)| <b>@deprecated.</b> Please use the 'exportHiddenWorksheet' property instead. Indicating if exporting the hidden worksheet content.The default value is true. |
| [setExportHiddenWorksheet(boolean)](#setExportHiddenWorksheet-boolean-)| <b>@deprecated.</b> Please use the 'exportHiddenWorksheet' property instead. Indicating if exporting the hidden worksheet content.The default value is true. |
| [getPresentationPreference()](#getPresentationPreference--)| <b>@deprecated.</b> Please use the 'presentationPreference' property instead. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [setPresentationPreference(boolean)](#setPresentationPreference-boolean-)| <b>@deprecated.</b> Please use the 'presentationPreference' property instead. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true. |
| [getCellCssPrefix()](#getCellCssPrefix--)| <b>@deprecated.</b> Please use the 'cellCssPrefix' property instead. Gets and sets the prefix of the css name,the default value is "". |
| [setCellCssPrefix(string)](#setCellCssPrefix-string-)| <b>@deprecated.</b> Please use the 'cellCssPrefix' property instead. Gets and sets the prefix of the css name,the default value is "". |
| [getTableCssId()](#getTableCssId--)| <b>@deprecated.</b> Please use the 'tableCssId' property instead. Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [setTableCssId(string)](#setTableCssId-string-)| <b>@deprecated.</b> Please use the 'tableCssId' property instead. Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [isFullPathLink()](#isFullPathLink--)| <b>@deprecated.</b> Please use the 'isFullPathLink' property instead. Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [setIsFullPathLink(boolean)](#setIsFullPathLink-boolean-)| <b>@deprecated.</b> Please use the 'isFullPathLink' property instead. Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--)| <b>@deprecated.</b> Please use the 'exportWorksheetCSSSeparately' property instead. Indicating whether export the worksheet css separately.The default value is false. |
| [setExportWorksheetCSSSeparately(boolean)](#setExportWorksheetCSSSeparately-boolean-)| <b>@deprecated.</b> Please use the 'exportWorksheetCSSSeparately' property instead. Indicating whether export the worksheet css separately.The default value is false. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--)| <b>@deprecated.</b> Please use the 'exportSimilarBorderStyle' property instead. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [setExportSimilarBorderStyle(boolean)](#setExportSimilarBorderStyle-boolean-)| <b>@deprecated.</b> Please use the 'exportSimilarBorderStyle' property instead. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--)| <b>@deprecated.</b> Please use the 'mergeEmptyTdForcely' property instead. Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [setMergeEmptyTdForcely(boolean)](#setMergeEmptyTdForcely-boolean-)| <b>@deprecated.</b> Please use the 'mergeEmptyTdForcely' property instead. Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--)| <b>@deprecated.</b> Please use the 'mergeEmptyTdType' property instead. The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [setMergeEmptyTdType(MergeEmptyTdType)](#setMergeEmptyTdType-mergeemptytdtype-)| <b>@deprecated.</b> Please use the 'mergeEmptyTdType' property instead. The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. |
| [getExportCellCoordinate()](#getExportCellCoordinate--)| <b>@deprecated.</b> Please use the 'exportCellCoordinate' property instead. Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [setExportCellCoordinate(boolean)](#setExportCellCoordinate-boolean-)| <b>@deprecated.</b> Please use the 'exportCellCoordinate' property instead. Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [getExportExtraHeadings()](#getExportExtraHeadings--)| <b>@deprecated.</b> Please use the 'exportExtraHeadings' property instead. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [setExportExtraHeadings(boolean)](#setExportExtraHeadings-boolean-)| <b>@deprecated.</b> Please use the 'exportExtraHeadings' property instead. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--)| <b>@deprecated.</b> Please use the 'exportRowColumnHeadings' property instead. Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [setExportRowColumnHeadings(boolean)](#setExportRowColumnHeadings-boolean-)| <b>@deprecated.</b> Please use the 'exportRowColumnHeadings' property instead. Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [getExportFormula()](#getExportFormula--)| <b>@deprecated.</b> Please use the 'exportFormula' property instead. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [setExportFormula(boolean)](#setExportFormula-boolean-)| <b>@deprecated.</b> Please use the 'exportFormula' property instead. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [getAddTooltipText()](#getAddTooltipText--)| <b>@deprecated.</b> Please use the 'addTooltipText' property instead. Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [setAddTooltipText(boolean)](#setAddTooltipText-boolean-)| <b>@deprecated.</b> Please use the 'addTooltipText' property instead. Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [getExportGridLines()](#getExportGridLines--)| <b>@deprecated.</b> Please use the 'exportGridLines' property instead. Indicating whether exporting the gridlines.The default value is false. |
| [setExportGridLines(boolean)](#setExportGridLines-boolean-)| <b>@deprecated.</b> Please use the 'exportGridLines' property instead. Indicating whether exporting the gridlines.The default value is false. |
| [getExportBogusRowData()](#getExportBogusRowData--)| <b>@deprecated.</b> Please use the 'exportBogusRowData' property instead. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportBogusRowData(boolean)](#setExportBogusRowData-boolean-)| <b>@deprecated.</b> Please use the 'exportBogusRowData' property instead. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--)| <b>@deprecated.</b> Please use the 'excludeUnusedStyles' property instead. Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [setExcludeUnusedStyles(boolean)](#setExcludeUnusedStyles-boolean-)| <b>@deprecated.</b> Please use the 'excludeUnusedStyles' property instead. Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [getExportDocumentProperties()](#getExportDocumentProperties--)| <b>@deprecated.</b> Please use the 'exportDocumentProperties' property instead. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportDocumentProperties(boolean)](#setExportDocumentProperties-boolean-)| <b>@deprecated.</b> Please use the 'exportDocumentProperties' property instead. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--)| <b>@deprecated.</b> Please use the 'exportWorksheetProperties' property instead. Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportWorksheetProperties(boolean)](#setExportWorksheetProperties-boolean-)| <b>@deprecated.</b> Please use the 'exportWorksheetProperties' property instead. Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--)| <b>@deprecated.</b> Please use the 'exportWorkbookProperties' property instead. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportWorkbookProperties(boolean)](#setExportWorkbookProperties-boolean-)| <b>@deprecated.</b> Please use the 'exportWorkbookProperties' property instead. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--)| <b>@deprecated.</b> Please use the 'exportFrameScriptsAndProperties' property instead. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [setExportFrameScriptsAndProperties(boolean)](#setExportFrameScriptsAndProperties-boolean-)| <b>@deprecated.</b> Please use the 'exportFrameScriptsAndProperties' property instead. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [getExportDataOptions()](#getExportDataOptions--)| <b>@deprecated.</b> Please use the 'exportDataOptions' property instead. Indicating the rule of exporting html file data.The default value is All. |
| [setExportDataOptions(HtmlExportDataOptions)](#setExportDataOptions-htmlexportdataoptions-)| <b>@deprecated.</b> Please use the 'exportDataOptions' property instead. Indicating the rule of exporting html file data.The default value is All. |
| [getLinkTargetType()](#getLinkTargetType--)| <b>@deprecated.</b> Please use the 'linkTargetType' property instead. Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
| [setLinkTargetType(HtmlLinkTargetType)](#setLinkTargetType-htmllinktargettype-)| <b>@deprecated.</b> Please use the 'linkTargetType' property instead. Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
| [isIECompatible()](#isIECompatible--)| <b>@deprecated.</b> Please use the 'isIECompatible' property instead. Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [setIsIECompatible(boolean)](#setIsIECompatible-boolean-)| <b>@deprecated.</b> Please use the 'isIECompatible' property instead. Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--)| <b>@deprecated.</b> Please use the 'formatDataIgnoreColumnWidth' property instead. Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [setFormatDataIgnoreColumnWidth(boolean)](#setFormatDataIgnoreColumnWidth-boolean-)| <b>@deprecated.</b> Please use the 'formatDataIgnoreColumnWidth' property instead. Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false. |
| [getCalculateFormula()](#getCalculateFormula--)| <b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving html file. |
| [setCalculateFormula(boolean)](#setCalculateFormula-boolean-)| <b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving html file. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--)| <b>@deprecated.</b> Please use the 'isJsBrowserCompatible' property instead. Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [setIsJsBrowserCompatible(boolean)](#setIsJsBrowserCompatible-boolean-)| <b>@deprecated.</b> Please use the 'isJsBrowserCompatible' property instead. Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [isMobileCompatible()](#isMobileCompatible--)| <b>@deprecated.</b> Please use the 'isMobileCompatible' property instead. Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [setIsMobileCompatible(boolean)](#setIsMobileCompatible-boolean-)| <b>@deprecated.</b> Please use the 'isMobileCompatible' property instead. Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [getCssStyles()](#getCssStyles--)| <b>@deprecated.</b> Please use the 'cssStyles' property instead. Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example> |
| [setCssStyles(string)](#setCssStyles-string-)| <b>@deprecated.</b> Please use the 'cssStyles' property instead. Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example> |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--)| <b>@deprecated.</b> Please use the 'hideOverflowWrappedText' property instead. Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [setHideOverflowWrappedText(boolean)](#setHideOverflowWrappedText-boolean-)| <b>@deprecated.</b> Please use the 'hideOverflowWrappedText' property instead. Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [isBorderCollapsed()](#isBorderCollapsed--)| <b>@deprecated.</b> Please use the 'isBorderCollapsed' property instead. Indicates whether the table borders are collapsed. The default value is true. |
| [setIsBorderCollapsed(boolean)](#setIsBorderCollapsed-boolean-)| <b>@deprecated.</b> Please use the 'isBorderCollapsed' property instead. Indicates whether the table borders are collapsed. The default value is true. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--)| <b>@deprecated.</b> Please use the 'encodeEntityAsCode' property instead. Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [setEncodeEntityAsCode(boolean)](#setEncodeEntityAsCode-boolean-)| <b>@deprecated.</b> Please use the 'encodeEntityAsCode' property instead. Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--)| <b>@deprecated.</b> Please use the 'officeMathOutputMode' property instead. Indicates how OfficeMath objects are exported to HTML, Default value is Image. |
| [setOfficeMathOutputMode(HtmlOfficeMathOutputType)](#setOfficeMathOutputMode-htmlofficemathoutputtype-)| <b>@deprecated.</b> Please use the 'officeMathOutputMode' property instead. Indicates how OfficeMath objects are exported to HTML, Default value is Image. |
| [getCellNameAttribute()](#getCellNameAttribute--)| <b>@deprecated.</b> Please use the 'cellNameAttribute' property instead. Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [setCellNameAttribute(string)](#setCellNameAttribute-string-)| <b>@deprecated.</b> Please use the 'cellNameAttribute' property instead. Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null. |
| [getDisableCss()](#getDisableCss--)| <b>@deprecated.</b> Please use the 'disableCss' property instead. Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [setDisableCss(boolean)](#setDisableCss-boolean-)| <b>@deprecated.</b> Please use the 'disableCss' property instead. Indicates whether only inline styles are applied, without relying on CSS. The default value is false. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--)| <b>@deprecated.</b> Please use the 'enableCssCustomProperties' property instead. Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [setEnableCssCustomProperties(boolean)](#setEnableCssCustomProperties-boolean-)| <b>@deprecated.</b> Please use the 'enableCssCustomProperties' property instead. Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false. |
| [getHtmlVersion()](#getHtmlVersion--)| <b>@deprecated.</b> Please use the 'htmlVersion' property instead. Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default. |
| [setHtmlVersion(HtmlVersion)](#setHtmlVersion-htmlversion-)| <b>@deprecated.</b> Please use the 'htmlVersion' property instead. Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default. |
| [getSheetSet()](#getSheetSet--)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [setSheetSet(SheetSet)](#setSheetSet-sheetset-)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [getLayoutMode()](#getLayoutMode--)| <b>@deprecated.</b> Please use the 'layoutMode' property instead. Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/) |
| [setLayoutMode(HtmlLayoutMode)](#setLayoutMode-htmllayoutmode-)| <b>@deprecated.</b> Please use the 'layoutMode' property instead. Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/) |
| [getEmbeddedFontType()](#getEmbeddedFontType--)| <b>@deprecated.</b> Please use the 'embeddedFontType' property instead. Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html. |
| [setEmbeddedFontType(HtmlEmbeddedFontType)](#setEmbeddedFontType-htmlembeddedfonttype-)| <b>@deprecated.</b> Please use the 'embeddedFontType' property instead. Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--)| <b>@deprecated.</b> Please use the 'exportNamedRangeAnchors' property instead. Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true. |
| [setExportNamedRangeAnchors(boolean)](#setExportNamedRangeAnchors-boolean-)| <b>@deprecated.</b> Please use the 'exportNamedRangeAnchors' property instead. Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true. |
| [getDataBarRenderMode()](#getDataBarRenderMode--)| <b>@deprecated.</b> Please use the 'dataBarRenderMode' property instead. Represents the mode of how to render DataBar when converting Excel files to html files. Default value is [DataBarRenderMode.BackgroundColor](../databarrendermode.backgroundcolor/). |
| [setDataBarRenderMode(DataBarRenderMode)](#setDataBarRenderMode-databarrendermode-)| <b>@deprecated.</b> Please use the 'dataBarRenderMode' property instead. Represents the mode of how to render DataBar when converting Excel files to html files. Default value is [DataBarRenderMode.BackgroundColor](../databarrendermode.backgroundcolor/). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveFormat()](#getSaveFormat--)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets the save file format. |
| [getClearData()](#getClearData--)| <b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file. |
| [setClearData(boolean)](#setClearData-boolean-)| <b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file. |
| [getCachedFileFolder()](#getCachedFileFolder--)| <b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache. |
| [setCachedFileFolder(string)](#setCachedFileFolder-string-)| <b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache. |
| [getValidateMergedAreas()](#getValidateMergedAreas--)| <b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file. |
| [setValidateMergedAreas(boolean)](#setValidateMergedAreas-boolean-)| <b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file. |
| [getMergeAreas()](#getMergeAreas--)| <b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeAreas(boolean)](#setMergeAreas-boolean-)| <b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getCreateDirectory()](#getCreateDirectory--)| <b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreateDirectory(boolean)](#setCreateDirectory-boolean-)| <b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getSortNames()](#getSortNames--)| <b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file. |
| [setSortNames(boolean)](#setSortNames-boolean-)| <b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file. |
| [getSortExternalNames()](#getSortExternalNames--)| <b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file. |
| [setSortExternalNames(boolean)](#setSortExternalNames-boolean-)| <b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file. |
| [getRefreshChartCache()](#getRefreshChartCache--)| <b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data |
| [setRefreshChartCache(boolean)](#setRefreshChartCache-boolean-)| <b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| <b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| <b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| <b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| <b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true. |


### constructor() {#constructor--}

Creates options for saving html file.

```javascript
constructor();
```


### constructor(SaveOptions) {#constructor-saveoptions-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: SaveOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | SaveOptions | The parent object. |

### constructor(SaveFormat) {#constructor-saveformat-}

Creates options for saving htm file.

```javascript
constructor(saveFormat: SaveFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be one of following types: [SaveFormat.Html](../saveformat.html/)  or [SaveFormat.MHtml](../saveformat.mhtml/),         /// otherwise the saved format will be set as [SaveFormat.Html](../saveformat.html/) automatically. |

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

Indicates how OfficeMath objects are exported to HTML, Default value is Image.

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


### exportNamedRangeAnchors {#exportNamedRangeAnchors--}

Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true.

```javascript
exportNamedRangeAnchors : boolean;
```


### dataBarRenderMode {#dataBarRenderMode--}

Represents the mode of how to render DataBar when converting Excel files to html files. Default value is [DataBarRenderMode.BackgroundColor](../databarrendermode.backgroundcolor/).

```javascript
dataBarRenderMode : DataBarRenderMode;
```


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

### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}

<b>@deprecated.</b> Please use the 'ignoreInvisibleShapes' property instead. Indicate whether exporting those not visible shapes

```javascript
getIgnoreInvisibleShapes() : boolean;
```


**Remarks**

The default values is false.

### setIgnoreInvisibleShapes(boolean) {#setIgnoreInvisibleShapes-boolean-}

<b>@deprecated.</b> Please use the 'ignoreInvisibleShapes' property instead. Indicate whether exporting those not visible shapes

```javascript
setIgnoreInvisibleShapes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default values is false.

### getPageTitle() {#getPageTitle--}

<b>@deprecated.</b> Please use the 'pageTitle' property instead. The title of the html page. Only for saving to html stream.

```javascript
getPageTitle() : string;
```


### setPageTitle(string) {#setPageTitle-string-}

<b>@deprecated.</b> Please use the 'pageTitle' property instead. The title of the html page. Only for saving to html stream.

```javascript
setPageTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}

<b>@deprecated.</b> Please use the 'attachedFilesDirectory' property instead. The directory that the attached files will be saved to. Only for saving to html stream.

```javascript
getAttachedFilesDirectory() : string;
```


### setAttachedFilesDirectory(string) {#setAttachedFilesDirectory-string-}

<b>@deprecated.</b> Please use the 'attachedFilesDirectory' property instead. The directory that the attached files will be saved to. Only for saving to html stream.

```javascript
setAttachedFilesDirectory(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}

<b>@deprecated.</b> Please use the 'attachedFilesUrlPrefix' property instead. Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

```javascript
getAttachedFilesUrlPrefix() : string;
```


### setAttachedFilesUrlPrefix(string) {#setAttachedFilesUrlPrefix-string-}

<b>@deprecated.</b> Please use the 'attachedFilesUrlPrefix' property instead. Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

```javascript
setAttachedFilesUrlPrefix(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDefaultFontName() {#getDefaultFontName--}

<b>@deprecated.</b> Please use the 'defaultFontName' property instead. Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```javascript
getDefaultFontName() : string;
```


### setDefaultFontName(string) {#setDefaultFontName-string-}

<b>@deprecated.</b> Please use the 'defaultFontName' property instead. Specify the default font name for exporting html, the default font will be used  when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```javascript
setDefaultFontName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAddGenericFont() {#getAddGenericFont--}

<b>@deprecated.</b> Please use the 'addGenericFont' property instead. Indicates whether to add a generic font to CSS font-family. The default value is true

```javascript
getAddGenericFont() : boolean;
```


### setAddGenericFont(boolean) {#setAddGenericFont-boolean-}

<b>@deprecated.</b> Please use the 'addGenericFont' property instead. Indicates whether to add a generic font to CSS font-family. The default value is true

```javascript
setAddGenericFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWorksheetScalable() {#getWorksheetScalable--}

<b>@deprecated.</b> Please use the 'worksheetScalable' property instead. Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```javascript
getWorksheetScalable() : boolean;
```


### setWorksheetScalable(boolean) {#setWorksheetScalable-boolean-}

<b>@deprecated.</b> Please use the 'worksheetScalable' property instead. Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```javascript
setWorksheetScalable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isExportComments() {#isExportComments--}

<b>@deprecated.</b> Please use the 'isExportComments' property instead. Indicates if exporting comments when saving file to html, the default value is false.

```javascript
isExportComments() : boolean;
```


### setIsExportComments(boolean) {#setIsExportComments-boolean-}

<b>@deprecated.</b> Please use the 'isExportComments' property instead. Indicates if exporting comments when saving file to html, the default value is false.

```javascript
setIsExportComments(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportCommentsType() {#getExportCommentsType--}

<b>@deprecated.</b> Please use the 'exportCommentsType' property instead. Represents type of exporting comments to html files.

```javascript
getExportCommentsType() : PrintCommentsType;
```


**Returns**

[PrintCommentsType](../printcommentstype/)

### setExportCommentsType(PrintCommentsType) {#setExportCommentsType-printcommentstype-}

<b>@deprecated.</b> Please use the 'exportCommentsType' property instead. Represents type of exporting comments to html files.

```javascript
setExportCommentsType(value: PrintCommentsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintCommentsType](../printcommentstype/) | The value to set. |

### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}

<b>@deprecated.</b> Please use the 'disableDownlevelRevealedComments' property instead. Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

```javascript
getDisableDownlevelRevealedComments() : boolean;
```


### setDisableDownlevelRevealedComments(boolean) {#setDisableDownlevelRevealedComments-boolean-}

<b>@deprecated.</b> Please use the 'disableDownlevelRevealedComments' property instead. Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

```javascript
setDisableDownlevelRevealedComments(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isExpImageToTempDir() {#isExpImageToTempDir--}

<b>@deprecated.</b> Please use the 'isExpImageToTempDir' property instead. Indicates whether exporting image files to temp directory. Only for saving to html stream.

```javascript
isExpImageToTempDir() : boolean;
```


### setIsExpImageToTempDir(boolean) {#setIsExpImageToTempDir-boolean-}

<b>@deprecated.</b> Please use the 'isExpImageToTempDir' property instead. Indicates whether exporting image files to temp directory. Only for saving to html stream.

```javascript
setIsExpImageToTempDir(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getImageScalable() {#getImageScalable--}

<b>@deprecated.</b> Please use the 'imageScalable' property instead. Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

```javascript
getImageScalable() : boolean;
```


### setImageScalable(boolean) {#setImageScalable-boolean-}

<b>@deprecated.</b> Please use the 'imageScalable' property instead. Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

```javascript
setImageScalable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWidthScalable() {#getWidthScalable--}

<b>@deprecated.</b> Please use the 'widthScalable' property instead. Indicates whether exporting column width in unit of scale to html. The default value is false.

```javascript
getWidthScalable() : boolean;
```


### setWidthScalable(boolean) {#setWidthScalable-boolean-}

<b>@deprecated.</b> Please use the 'widthScalable' property instead. Indicates whether exporting column width in unit of scale to html. The default value is false.

```javascript
setWidthScalable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportSingleTab() {#getExportSingleTab--}

<b>@deprecated.</b> Please use the 'exportSingleTab' property instead. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```javascript
getExportSingleTab() : boolean;
```


### setExportSingleTab(boolean) {#setExportSingleTab-boolean-}

<b>@deprecated.</b> Please use the 'exportSingleTab' property instead. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```javascript
setExportSingleTab(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportImagesAsBase64() {#getExportImagesAsBase64--}

<b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.

```javascript
getExportImagesAsBase64() : boolean;
```


**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### setExportImagesAsBase64(boolean) {#setExportImagesAsBase64-boolean-}

<b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.

```javascript
setExportImagesAsBase64(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}

<b>@deprecated.</b> Please use the 'exportActiveWorksheetOnly' property instead. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```javascript
getExportActiveWorksheetOnly() : boolean;
```


### setExportActiveWorksheetOnly(boolean) {#setExportActiveWorksheetOnly-boolean-}

<b>@deprecated.</b> Please use the 'exportActiveWorksheetOnly' property instead. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```javascript
setExportActiveWorksheetOnly(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}

<b>@deprecated.</b> Please use the 'exportPrintAreaOnly' property instead. Indicates if only exporting the print area to html file. The default value is false.

```javascript
getExportPrintAreaOnly() : boolean;
```


### setExportPrintAreaOnly(boolean) {#setExportPrintAreaOnly-boolean-}

<b>@deprecated.</b> Please use the 'exportPrintAreaOnly' property instead. Indicates if only exporting the print area to html file. The default value is false.

```javascript
setExportPrintAreaOnly(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportArea() {#getExportArea--}

<b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```javascript
getExportArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### setExportArea(CellArea) {#setExportArea-cellarea-}

<b>@deprecated.</b> Please use the 'exportArea' property instead. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```javascript
setExportArea(value: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../cellarea/) | The value to set. |

### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}

<b>@deprecated.</b> Please use the 'parseHtmlTagInCell' property instead. Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true.

```javascript
getParseHtmlTagInCell() : boolean;
```


### setParseHtmlTagInCell(boolean) {#setParseHtmlTagInCell-boolean-}

<b>@deprecated.</b> Please use the 'parseHtmlTagInCell' property instead. Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is. The default value is true.

```javascript
setParseHtmlTagInCell(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHtmlCrossStringType() {#getHtmlCrossStringType--}

<b>@deprecated.</b> Please use the 'htmlCrossStringType' property instead. Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```javascript
getHtmlCrossStringType() : HtmlCrossType;
```


**Returns**

[HtmlCrossType](../htmlcrosstype/)

### setHtmlCrossStringType(HtmlCrossType) {#setHtmlCrossStringType-htmlcrosstype-}

<b>@deprecated.</b> Please use the 'htmlCrossStringType' property instead. Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.

```javascript
setHtmlCrossStringType(value: HtmlCrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlCrossType](../htmlcrosstype/) | The value to set. |

### getHiddenColDisplayType() {#getHiddenColDisplayType--}

<b>@deprecated.</b> Please use the 'hiddenColDisplayType' property instead. Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

```javascript
getHiddenColDisplayType() : HtmlHiddenColDisplayType;
```


**Returns**

[HtmlHiddenColDisplayType](../htmlhiddencoldisplaytype/)

### setHiddenColDisplayType(HtmlHiddenColDisplayType) {#setHiddenColDisplayType-htmlhiddencoldisplaytype-}

<b>@deprecated.</b> Please use the 'hiddenColDisplayType' property instead. Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

```javascript
setHiddenColDisplayType(value: HtmlHiddenColDisplayType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlHiddenColDisplayType](../htmlhiddencoldisplaytype/) | The value to set. |

### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}

<b>@deprecated.</b> Please use the 'hiddenRowDisplayType' property instead. Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```javascript
getHiddenRowDisplayType() : HtmlHiddenRowDisplayType;
```


**Returns**

[HtmlHiddenRowDisplayType](../htmlhiddenrowdisplaytype/)

### setHiddenRowDisplayType(HtmlHiddenRowDisplayType) {#setHiddenRowDisplayType-htmlhiddenrowdisplaytype-}

<b>@deprecated.</b> Please use the 'hiddenRowDisplayType' property instead. Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```javascript
setHiddenRowDisplayType(value: HtmlHiddenRowDisplayType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlHiddenRowDisplayType](../htmlhiddenrowdisplaytype/) | The value to set. |

### getEncoding() {#getEncoding--}

<b>@deprecated.</b> Please use the 'encoding' property instead. If not set,use Encoding.UTF8 as default enconding type.

```javascript
getEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setEncoding(EncodingType) {#setEncoding-encodingtype-}

<b>@deprecated.</b> Please use the 'encoding' property instead. If not set,use Encoding.UTF8 as default enconding type.

```javascript
setEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### getFilePathProvider() {#getFilePathProvider--}

<b>@deprecated.</b> Please use the 'filePathProvider' property instead. Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

```javascript
getFilePathProvider() : IFilePathProvider;
```


**Returns**

[IFilePathProvider](../ifilepathprovider/)

### setFilePathProvider(IFilePathProvider) {#setFilePathProvider-ifilepathprovider-}

<b>@deprecated.</b> Please use the 'filePathProvider' property instead. Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

```javascript
setFilePathProvider(value: IFilePathProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFilePathProvider](../ifilepathprovider/) | The value to set. |

### getImageOptions() {#getImageOptions--}

<b>@deprecated.</b> Please use the 'imageOptions' property instead. Get the ImageOrPrintOptions object before exporting

```javascript
getImageOptions() : ImageOrPrintOptions;
```


**Returns**

[ImageOrPrintOptions](../imageorprintoptions/)

### getSaveAsSingleFile() {#getSaveAsSingleFile--}

<b>@deprecated.</b> Please use the 'saveAsSingleFile' property instead. Indicates whether save the html as single file. The default value is false.

```javascript
getSaveAsSingleFile() : boolean;
```


**Remarks**

If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### setSaveAsSingleFile(boolean) {#setSaveAsSingleFile-boolean-}

<b>@deprecated.</b> Please use the 'saveAsSingleFile' property instead. Indicates whether save the html as single file. The default value is false.

```javascript
setSaveAsSingleFile(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### getShowAllSheets() {#getShowAllSheets--}

<b>@deprecated.</b> Please use the 'showAllSheets' property instead. Indicates whether showing all sheets when saving  as a single html file.

```javascript
getShowAllSheets() : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### setShowAllSheets(boolean) {#setShowAllSheets-boolean-}

<b>@deprecated.</b> Please use the 'showAllSheets' property instead. Indicates whether showing all sheets when saving  as a single html file.

```javascript
setShowAllSheets(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### getExportPageHeaders() {#getExportPageHeaders--}

<b>@deprecated.</b> Please use the 'exportPageHeaders' property instead. Indicates whether exporting page headers.

```javascript
getExportPageHeaders() : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### setExportPageHeaders(boolean) {#setExportPageHeaders-boolean-}

<b>@deprecated.</b> Please use the 'exportPageHeaders' property instead. Indicates whether exporting page headers.

```javascript
setExportPageHeaders(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### getExportPageFooters() {#getExportPageFooters--}

<b>@deprecated.</b> Please use the 'exportPageFooters' property instead. Indicates whether exporting page headers.

```javascript
getExportPageFooters() : boolean;
```


**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### setExportPageFooters(boolean) {#setExportPageFooters-boolean-}

<b>@deprecated.</b> Please use the 'exportPageFooters' property instead. Indicates whether exporting page headers.

```javascript
setExportPageFooters(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [SaveAsSingleFile](../saveassinglefile/) is True.

### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}

<b>@deprecated.</b> Please use the 'exportHiddenWorksheet' property instead. Indicating if exporting the hidden worksheet content.The default value is true.

```javascript
getExportHiddenWorksheet() : boolean;
```


### setExportHiddenWorksheet(boolean) {#setExportHiddenWorksheet-boolean-}

<b>@deprecated.</b> Please use the 'exportHiddenWorksheet' property instead. Indicating if exporting the hidden worksheet content.The default value is true.

```javascript
setExportHiddenWorksheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPresentationPreference() {#getPresentationPreference--}

<b>@deprecated.</b> Please use the 'presentationPreference' property instead. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```javascript
getPresentationPreference() : boolean;
```


### setPresentationPreference(boolean) {#setPresentationPreference-boolean-}

<b>@deprecated.</b> Please use the 'presentationPreference' property instead. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```javascript
setPresentationPreference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCellCssPrefix() {#getCellCssPrefix--}

<b>@deprecated.</b> Please use the 'cellCssPrefix' property instead. Gets and sets the prefix of the css name,the default value is "".

```javascript
getCellCssPrefix() : string;
```


### setCellCssPrefix(string) {#setCellCssPrefix-string-}

<b>@deprecated.</b> Please use the 'cellCssPrefix' property instead. Gets and sets the prefix of the css name,the default value is "".

```javascript
setCellCssPrefix(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTableCssId() {#getTableCssId--}

<b>@deprecated.</b> Please use the 'tableCssId' property instead. Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```javascript
getTableCssId() : string;
```


### setTableCssId(string) {#setTableCssId-string-}

<b>@deprecated.</b> Please use the 'tableCssId' property instead. Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```javascript
setTableCssId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isFullPathLink() {#isFullPathLink--}

<b>@deprecated.</b> Please use the 'isFullPathLink' property instead. Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

```javascript
isFullPathLink() : boolean;
```


### setIsFullPathLink(boolean) {#setIsFullPathLink-boolean-}

<b>@deprecated.</b> Please use the 'isFullPathLink' property instead. Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

```javascript
setIsFullPathLink(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}

<b>@deprecated.</b> Please use the 'exportWorksheetCSSSeparately' property instead. Indicating whether export the worksheet css separately.The default value is false.

```javascript
getExportWorksheetCSSSeparately() : boolean;
```


### setExportWorksheetCSSSeparately(boolean) {#setExportWorksheetCSSSeparately-boolean-}

<b>@deprecated.</b> Please use the 'exportWorksheetCSSSeparately' property instead. Indicating whether export the worksheet css separately.The default value is false.

```javascript
setExportWorksheetCSSSeparately(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}

<b>@deprecated.</b> Please use the 'exportSimilarBorderStyle' property instead. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```javascript
getExportSimilarBorderStyle() : boolean;
```


### setExportSimilarBorderStyle(boolean) {#setExportSimilarBorderStyle-boolean-}

<b>@deprecated.</b> Please use the 'exportSimilarBorderStyle' property instead. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

```javascript
setExportSimilarBorderStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}

<b>@deprecated.</b> Please use the 'mergeEmptyTdForcely' property instead. Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

```javascript
getMergeEmptyTdForcely() : boolean;
```


### setMergeEmptyTdForcely(boolean) {#setMergeEmptyTdForcely-boolean-}

<b>@deprecated.</b> Please use the 'mergeEmptyTdForcely' property instead. Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

```javascript
setMergeEmptyTdForcely(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMergeEmptyTdType() {#getMergeEmptyTdType--}

<b>@deprecated.</b> Please use the 'mergeEmptyTdType' property instead. The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.

```javascript
getMergeEmptyTdType() : MergeEmptyTdType;
```


**Returns**

[MergeEmptyTdType](../mergeemptytdtype/)

### setMergeEmptyTdType(MergeEmptyTdType) {#setMergeEmptyTdType-mergeemptytdtype-}

<b>@deprecated.</b> Please use the 'mergeEmptyTdType' property instead. The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default.

```javascript
setMergeEmptyTdType(value: MergeEmptyTdType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MergeEmptyTdType](../mergeemptytdtype/) | The value to set. |

### getExportCellCoordinate() {#getExportCellCoordinate--}

<b>@deprecated.</b> Please use the 'exportCellCoordinate' property instead. Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

```javascript
getExportCellCoordinate() : boolean;
```


### setExportCellCoordinate(boolean) {#setExportCellCoordinate-boolean-}

<b>@deprecated.</b> Please use the 'exportCellCoordinate' property instead. Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

```javascript
setExportCellCoordinate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportExtraHeadings() {#getExportExtraHeadings--}

<b>@deprecated.</b> Please use the 'exportExtraHeadings' property instead. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```javascript
getExportExtraHeadings() : boolean;
```


### setExportExtraHeadings(boolean) {#setExportExtraHeadings-boolean-}

<b>@deprecated.</b> Please use the 'exportExtraHeadings' property instead. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```javascript
setExportExtraHeadings(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}

<b>@deprecated.</b> Please use the 'exportRowColumnHeadings' property instead. Indicates whether exports sheet's row and column headings when saving to HTML files.

```javascript
getExportRowColumnHeadings() : boolean;
```


**Remarks**

The default value is false.

### setExportRowColumnHeadings(boolean) {#setExportRowColumnHeadings-boolean-}

<b>@deprecated.</b> Please use the 'exportRowColumnHeadings' property instead. Indicates whether exports sheet's row and column headings when saving to HTML files.

```javascript
setExportRowColumnHeadings(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getExportFormula() {#getExportFormula--}

<b>@deprecated.</b> Please use the 'exportFormula' property instead. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```javascript
getExportFormula() : boolean;
```


### setExportFormula(boolean) {#setExportFormula-boolean-}

<b>@deprecated.</b> Please use the 'exportFormula' property instead. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```javascript
setExportFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAddTooltipText() {#getAddTooltipText--}

<b>@deprecated.</b> Please use the 'addTooltipText' property instead. Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

```javascript
getAddTooltipText() : boolean;
```


### setAddTooltipText(boolean) {#setAddTooltipText-boolean-}

<b>@deprecated.</b> Please use the 'addTooltipText' property instead. Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

```javascript
setAddTooltipText(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportGridLines() {#getExportGridLines--}

<b>@deprecated.</b> Please use the 'exportGridLines' property instead. Indicating whether exporting the gridlines.The default value is false.

```javascript
getExportGridLines() : boolean;
```


### setExportGridLines(boolean) {#setExportGridLines-boolean-}

<b>@deprecated.</b> Please use the 'exportGridLines' property instead. Indicating whether exporting the gridlines.The default value is false.

```javascript
setExportGridLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportBogusRowData() {#getExportBogusRowData--}

<b>@deprecated.</b> Please use the 'exportBogusRowData' property instead. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportBogusRowData() : boolean;
```


### setExportBogusRowData(boolean) {#setExportBogusRowData-boolean-}

<b>@deprecated.</b> Please use the 'exportBogusRowData' property instead. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportBogusRowData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}

<b>@deprecated.</b> Please use the 'excludeUnusedStyles' property instead. Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

```javascript
getExcludeUnusedStyles() : boolean;
```


### setExcludeUnusedStyles(boolean) {#setExcludeUnusedStyles-boolean-}

<b>@deprecated.</b> Please use the 'excludeUnusedStyles' property instead. Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

```javascript
setExcludeUnusedStyles(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportDocumentProperties() {#getExportDocumentProperties--}

<b>@deprecated.</b> Please use the 'exportDocumentProperties' property instead. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportDocumentProperties() : boolean;
```


### setExportDocumentProperties(boolean) {#setExportDocumentProperties-boolean-}

<b>@deprecated.</b> Please use the 'exportDocumentProperties' property instead. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportDocumentProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportWorksheetProperties() {#getExportWorksheetProperties--}

<b>@deprecated.</b> Please use the 'exportWorksheetProperties' property instead. Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportWorksheetProperties() : boolean;
```


### setExportWorksheetProperties(boolean) {#setExportWorksheetProperties-boolean-}

<b>@deprecated.</b> Please use the 'exportWorksheetProperties' property instead. Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportWorksheetProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportWorkbookProperties() {#getExportWorkbookProperties--}

<b>@deprecated.</b> Please use the 'exportWorkbookProperties' property instead. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportWorkbookProperties() : boolean;
```


### setExportWorkbookProperties(boolean) {#setExportWorkbookProperties-boolean-}

<b>@deprecated.</b> Please use the 'exportWorkbookProperties' property instead. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportWorkbookProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}

<b>@deprecated.</b> Please use the 'exportFrameScriptsAndProperties' property instead. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
getExportFrameScriptsAndProperties() : boolean;
```


### setExportFrameScriptsAndProperties(boolean) {#setExportFrameScriptsAndProperties-boolean-}

<b>@deprecated.</b> Please use the 'exportFrameScriptsAndProperties' property instead. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```javascript
setExportFrameScriptsAndProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportDataOptions() {#getExportDataOptions--}

<b>@deprecated.</b> Please use the 'exportDataOptions' property instead. Indicating the rule of exporting html file data.The default value is All.

```javascript
getExportDataOptions() : HtmlExportDataOptions;
```


**Returns**

[HtmlExportDataOptions](../htmlexportdataoptions/)

### setExportDataOptions(HtmlExportDataOptions) {#setExportDataOptions-htmlexportdataoptions-}

<b>@deprecated.</b> Please use the 'exportDataOptions' property instead. Indicating the rule of exporting html file data.The default value is All.

```javascript
setExportDataOptions(value: HtmlExportDataOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlExportDataOptions](../htmlexportdataoptions/) | The value to set. |

### getLinkTargetType() {#getLinkTargetType--}

<b>@deprecated.</b> Please use the 'linkTargetType' property instead. Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent.

```javascript
getLinkTargetType() : HtmlLinkTargetType;
```


**Returns**

[HtmlLinkTargetType](../htmllinktargettype/)

### setLinkTargetType(HtmlLinkTargetType) {#setLinkTargetType-htmllinktargettype-}

<b>@deprecated.</b> Please use the 'linkTargetType' property instead. Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent.

```javascript
setLinkTargetType(value: HtmlLinkTargetType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlLinkTargetType](../htmllinktargettype/) | The value to set. |

### isIECompatible() {#isIECompatible--}

<b>@deprecated.</b> Please use the 'isIECompatible' property instead. Indicating whether the output HTML is compatible with IE browser. The defalut value is false

```javascript
isIECompatible() : boolean;
```


### setIsIECompatible(boolean) {#setIsIECompatible-boolean-}

<b>@deprecated.</b> Please use the 'isIECompatible' property instead. Indicating whether the output HTML is compatible with IE browser. The defalut value is false

```javascript
setIsIECompatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}

<b>@deprecated.</b> Please use the 'formatDataIgnoreColumnWidth' property instead. Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

```javascript
getFormatDataIgnoreColumnWidth() : boolean;
```


### setFormatDataIgnoreColumnWidth(boolean) {#setFormatDataIgnoreColumnWidth-boolean-}

<b>@deprecated.</b> Please use the 'formatDataIgnoreColumnWidth' property instead. Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

```javascript
setFormatDataIgnoreColumnWidth(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCalculateFormula() {#getCalculateFormula--}

<b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving html file.

```javascript
getCalculateFormula() : boolean;
```


**Remarks**

The default value is false.

### setCalculateFormula(boolean) {#setCalculateFormula-boolean-}

<b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving html file.

```javascript
setCalculateFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### isJsBrowserCompatible() {#isJsBrowserCompatible--}

<b>@deprecated.</b> Please use the 'isJsBrowserCompatible' property instead. Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

```javascript
isJsBrowserCompatible() : boolean;
```


### setIsJsBrowserCompatible(boolean) {#setIsJsBrowserCompatible-boolean-}

<b>@deprecated.</b> Please use the 'isJsBrowserCompatible' property instead. Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

```javascript
setIsJsBrowserCompatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isMobileCompatible() {#isMobileCompatible--}

<b>@deprecated.</b> Please use the 'isMobileCompatible' property instead. Indicates whether the output HTML is compatible with mobile devices. The default value is false.

```javascript
isMobileCompatible() : boolean;
```


### setIsMobileCompatible(boolean) {#setIsMobileCompatible-boolean-}

<b>@deprecated.</b> Please use the 'isMobileCompatible' property instead. Indicates whether the output HTML is compatible with mobile devices. The default value is false.

```javascript
setIsMobileCompatible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCssStyles() {#getCssStyles--}

<b>@deprecated.</b> Please use the 'cssStyles' property instead. Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example>

```javascript
getCssStyles() : string;
```


### setCssStyles(string) {#setCssStyles-string-}

<b>@deprecated.</b> Please use the 'cssStyles' property instead. Gets or sets the additional css styles for the formatter. Only works when [SaveAsSingleFile](../saveassinglefile/) is True. <example> CssStyles="body { padding: 5px }"; </example>

```javascript
setCssStyles(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}

<b>@deprecated.</b> Please use the 'hideOverflowWrappedText' property instead. Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

```javascript
getHideOverflowWrappedText() : boolean;
```


### setHideOverflowWrappedText(boolean) {#setHideOverflowWrappedText-boolean-}

<b>@deprecated.</b> Please use the 'hideOverflowWrappedText' property instead. Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

```javascript
setHideOverflowWrappedText(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isBorderCollapsed() {#isBorderCollapsed--}

<b>@deprecated.</b> Please use the 'isBorderCollapsed' property instead. Indicates whether the table borders are collapsed. The default value is true.

```javascript
isBorderCollapsed() : boolean;
```


### setIsBorderCollapsed(boolean) {#setIsBorderCollapsed-boolean-}

<b>@deprecated.</b> Please use the 'isBorderCollapsed' property instead. Indicates whether the table borders are collapsed. The default value is true.

```javascript
setIsBorderCollapsed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}

<b>@deprecated.</b> Please use the 'encodeEntityAsCode' property instead. Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false.

```javascript
getEncodeEntityAsCode() : boolean;
```


### setEncodeEntityAsCode(boolean) {#setEncodeEntityAsCode-boolean-}

<b>@deprecated.</b> Please use the 'encodeEntityAsCode' property instead. Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false.

```javascript
setEncodeEntityAsCode(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}

<b>@deprecated.</b> Please use the 'officeMathOutputMode' property instead. Indicates how OfficeMath objects are exported to HTML, Default value is Image.

```javascript
getOfficeMathOutputMode() : HtmlOfficeMathOutputType;
```


**Returns**

[HtmlOfficeMathOutputType](../htmlofficemathoutputtype/)

### setOfficeMathOutputMode(HtmlOfficeMathOutputType) {#setOfficeMathOutputMode-htmlofficemathoutputtype-}

<b>@deprecated.</b> Please use the 'officeMathOutputMode' property instead. Indicates how OfficeMath objects are exported to HTML, Default value is Image.

```javascript
setOfficeMathOutputMode(value: HtmlOfficeMathOutputType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlOfficeMathOutputType](../htmlofficemathoutputtype/) | The value to set. |

### getCellNameAttribute() {#getCellNameAttribute--}

<b>@deprecated.</b> Please use the 'cellNameAttribute' property instead. Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```javascript
getCellNameAttribute() : string;
```


### setCellNameAttribute(string) {#setCellNameAttribute-string-}

<b>@deprecated.</b> Please use the 'cellNameAttribute' property instead. Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```javascript
setCellNameAttribute(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDisableCss() {#getDisableCss--}

<b>@deprecated.</b> Please use the 'disableCss' property instead. Indicates whether only inline styles are applied, without relying on CSS. The default value is false.

```javascript
getDisableCss() : boolean;
```


### setDisableCss(boolean) {#setDisableCss-boolean-}

<b>@deprecated.</b> Please use the 'disableCss' property instead. Indicates whether only inline styles are applied, without relying on CSS. The default value is false.

```javascript
setDisableCss(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}

<b>@deprecated.</b> Please use the 'enableCssCustomProperties' property instead. Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false.

```javascript
getEnableCssCustomProperties() : boolean;
```


### setEnableCssCustomProperties(boolean) {#setEnableCssCustomProperties-boolean-}

<b>@deprecated.</b> Please use the 'enableCssCustomProperties' property instead. Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false.

```javascript
setEnableCssCustomProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHtmlVersion() {#getHtmlVersion--}

<b>@deprecated.</b> Please use the 'htmlVersion' property instead. Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default.

```javascript
getHtmlVersion() : HtmlVersion;
```


**Returns**

[HtmlVersion](../htmlversion/)

### setHtmlVersion(HtmlVersion) {#setHtmlVersion-htmlversion-}

<b>@deprecated.</b> Please use the 'htmlVersion' property instead. Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default.

```javascript
setHtmlVersion(value: HtmlVersion) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlVersion](../htmlversion/) | The value to set. |

### getSheetSet() {#getSheetSet--}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
getSheetSet() : SheetSet;
```


**Returns**

[SheetSet](../sheetset/)

### setSheetSet(SheetSet) {#setSheetSet-sheetset-}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
setSheetSet(value: SheetSet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../sheetset/) | The value to set. |

### getLayoutMode() {#getLayoutMode--}

<b>@deprecated.</b> Please use the 'layoutMode' property instead. Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/)

```javascript
getLayoutMode() : HtmlLayoutMode;
```


**Returns**

[HtmlLayoutMode](../htmllayoutmode/)

### setLayoutMode(HtmlLayoutMode) {#setLayoutMode-htmllayoutmode-}

<b>@deprecated.</b> Please use the 'layoutMode' property instead. Gets or sets the layout mode when saving to HTML. The default value is [HtmlLayoutMode.Normal](../htmllayoutmode.normal/)

```javascript
setLayoutMode(value: HtmlLayoutMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlLayoutMode](../htmllayoutmode/) | The value to set. |

### getEmbeddedFontType() {#getEmbeddedFontType--}

<b>@deprecated.</b> Please use the 'embeddedFontType' property instead. Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html.

```javascript
getEmbeddedFontType() : HtmlEmbeddedFontType;
```


**Returns**

[HtmlEmbeddedFontType](../htmlembeddedfonttype/)

### setEmbeddedFontType(HtmlEmbeddedFontType) {#setEmbeddedFontType-htmlembeddedfonttype-}

<b>@deprecated.</b> Please use the 'embeddedFontType' property instead. Gets or sets the type of embedding font file into html file. Default value is [HtmlEmbeddedFontType.None](../htmlembeddedfonttype.none/) which indicates that no font will be embedded in html.

```javascript
setEmbeddedFontType(value: HtmlEmbeddedFontType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlEmbeddedFontType](../htmlembeddedfonttype/) | The value to set. |

### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}

<b>@deprecated.</b> Please use the 'exportNamedRangeAnchors' property instead. Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true.

```javascript
getExportNamedRangeAnchors() : boolean;
```


### setExportNamedRangeAnchors(boolean) {#setExportNamedRangeAnchors-boolean-}

<b>@deprecated.</b> Please use the 'exportNamedRangeAnchors' property instead. Indicates whether to export anchor elements for named ranges when saving as HTML. Default value is true.

```javascript
setExportNamedRangeAnchors(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDataBarRenderMode() {#getDataBarRenderMode--}

<b>@deprecated.</b> Please use the 'dataBarRenderMode' property instead. Represents the mode of how to render DataBar when converting Excel files to html files. Default value is [DataBarRenderMode.BackgroundColor](../databarrendermode.backgroundcolor/).

```javascript
getDataBarRenderMode() : DataBarRenderMode;
```


**Returns**

[DataBarRenderMode](../databarrendermode/)

### setDataBarRenderMode(DataBarRenderMode) {#setDataBarRenderMode-databarrendermode-}

<b>@deprecated.</b> Please use the 'dataBarRenderMode' property instead. Represents the mode of how to render DataBar when converting Excel files to html files. Default value is [DataBarRenderMode.BackgroundColor](../databarrendermode.backgroundcolor/).

```javascript
setDataBarRenderMode(value: DataBarRenderMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarRenderMode](../databarrendermode/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getSaveFormat() {#getSaveFormat--}

<b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets the save file format.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### getClearData() {#getClearData--}

<b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file.

```javascript
getClearData() : boolean;
```


### setClearData(boolean) {#setClearData-boolean-}

<b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file.

```javascript
setClearData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCachedFileFolder() {#getCachedFileFolder--}

<b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache.

```javascript
getCachedFileFolder() : string;
```


**Remarks**

If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.

### setCachedFileFolder(string) {#setCachedFileFolder-string-}

<b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache.

```javascript
setCachedFileFolder(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.

### getValidateMergedAreas() {#getValidateMergedAreas--}

<b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file.

```javascript
getValidateMergedAreas() : boolean;
```


**Remarks**

The default value is false.

### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}

<b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file.

```javascript
setValidateMergedAreas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getMergeAreas() {#getMergeAreas--}

<b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
getMergeAreas() : boolean;
```


**Remarks**

The default value is false.

### setMergeAreas(boolean) {#setMergeAreas-boolean-}

<b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
setMergeAreas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getCreateDirectory() {#getCreateDirectory--}

<b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
getCreateDirectory() : boolean;
```


**Remarks**

The default value is false.

### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}

<b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
setCreateDirectory(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getSortNames() {#getSortNames--}

<b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file.

```javascript
getSortNames() : boolean;
```


### setSortNames(boolean) {#setSortNames-boolean-}

<b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file.

```javascript
setSortNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSortExternalNames() {#getSortExternalNames--}

<b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file.

```javascript
getSortExternalNames() : boolean;
```


### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}

<b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file.

```javascript
setSortExternalNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshChartCache() {#getRefreshChartCache--}

<b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data

```javascript
getRefreshChartCache() : boolean;
```


### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}

<b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data

```javascript
setRefreshChartCache(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getCheckExcelRestriction() {#getCheckExcelRestriction--}

<b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

<b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUpdateSmartArt() {#getUpdateSmartArt--}

<b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false.

```javascript
getUpdateSmartArt() : boolean;
```


**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}

<b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false.

```javascript
setUpdateSmartArt(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}

<b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
getEncryptDocumentProperties() : boolean;
```


**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}

<b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
setEncryptDocumentProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.


