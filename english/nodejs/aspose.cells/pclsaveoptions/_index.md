---
title: "PclSaveOptions"
linktitle: "PclSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: ""
type: docs
weight: 2570
url: /nodejs/aspose.cells/pclsaveoptions/
---

## PclSaveOptions class

```js
new PclSaveOptions()
```

## Methods

| Name | Description |
| --- | --- |
| [addPrinterFont()](./addprinterfont/) |  |
| [getAllColumnsInOnePagePerSheet()](./getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [getCachedFileFolder()](./getcachedfilefolder/) | The cached file folder is used to store some large data. |
| [getCheckExcelRestriction()](./getcheckexcelrestriction/) |  |
| [getCheckFontCompatibility()](./getcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. The default value is true. Disable this prope |
| [getCheckWorkbookDefaultFont()](./getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [getClearData()](./getcleardata/) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getCustomRenderSettings()](./getcustomrendersettings/) |  |
| [getDefaultEditLanguage()](./getdefaulteditlanguage/) | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [getDefaultFont()](./getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [getDrawObjectEventHandler()](./getdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbedFont()](./getembedfont/) |  |
| [getEmfRenderSetting()](./getemfrendersetting/) | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [getEncryptDocumentProperties()](./getencryptdocumentproperties/) |  |
| [getGridlineColor()](./getgridlinecolor/) |  |
| [getGridlineType()](./getgridlinetype/) | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [getIgnoreError()](./getignoreerror/) | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [getMergeAreas()](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getOnePagePerSheet()](./getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [getOutputBlankPageWhenNothingToPrint()](./getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. Default is true. |
| [getPageCount()](./getpagecount/) | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.. |
| [getPageIndex()](./getpageindex/) | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [getPageSavingCallback()](./getpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [getPrintingPageType()](./getprintingpagetype/) | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in |
| [getRefreshChartCache()](./getrefreshchartcache/) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](./getsaveformat/) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSheetSet()](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. |
| [getSortExternalNames()](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](./getsortnames/) | Indicates whether sorting defined names before saving file. |
| [getTextCrossType()](./gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [getUpdateSmartArt()](./getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWarningCallback()](./getwarningcallback/) | Gets or sets warning callback. |
| [isFontSubstitutionCharGranularity()](./isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [setAllColumnsInOnePagePerSheet()](./setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [setCachedFileFolder()](./setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [setCheckExcelRestriction()](./setcheckexcelrestriction/) |  |
| [setCheckFontCompatibility()](./setcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. The default value is true. Disable this prope |
| [setCheckWorkbookDefaultFont()](./setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [setClearData()](./setcleardata/) | Make the workbook empty after saving the file. |
| [setCreateDirectory()](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setCustomRenderSettings()](./setcustomrendersettings/) |  |
| [setDefaultEditLanguage()](./setdefaulteditlanguage/) | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [setDefaultFont()](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [setDrawObjectEventHandler()](./setdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
| [setEmbedFont()](./setembedfont/) |  |
| [setEmfRenderSetting()](./setemfrendersetting/) | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [setEncryptDocumentProperties()](./setencryptdocumentproperties/) |  |
| [setFontSubstitutionCharGranularity()](./setfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [setGridlineColor()](./setgridlinecolor/) |  |
| [setGridlineType()](./setgridlinetype/) | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [setIgnoreError()](./setignoreerror/) | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [setMergeAreas()](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setOnePagePerSheet()](./setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [setOutputBlankPageWhenNothingToPrint()](./setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. Default is true. |
| [setPageCount()](./setpagecount/) | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.. |
| [setPageIndex()](./setpageindex/) | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [setPageSavingCallback()](./setpagesavingcallback/) | Control/Indicate progress of page saving process. |
| [setPrintingPageType()](./setprintingpagetype/) | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in |
| [setRefreshChartCache()](./setrefreshchartcache/) | Indicates whether refreshing chart cache data |
| [setSheetSet()](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. |
| [setSortExternalNames()](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](./setsortnames/) | Indicates whether sorting defined names before saving file. |
| [setTextCrossType()](./settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [setUpdateSmartArt()](./setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWarningCallback()](./setwarningcallback/) | Gets or sets warning callback. |
