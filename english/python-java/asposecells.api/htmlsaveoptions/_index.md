---
title: "HtmlSaveOptions Class"
linktitle: "HtmlSaveOptions"
articleTitle: "HtmlSaveOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the options for saving html file."
type: docs
weight: 2960
url: /python-java/asposecells.api/htmlsaveoptions/
---

## HtmlSaveOptions class

Represents the options for saving html file.

## Constructors

| Name | Description |
| --- | --- |
| [HtmlSaveOptions](#constructor) | Creates options for saving html file. |
| [HtmlSaveOptions](#constructor) | Creates options for saving htm file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IgnoreInvisibleShapes](#ignoreinvisibleshapes) | boolean | Indicate whether exporting those not visible shapes The default values is false. |
| [PageTitle](#pagetitle) | String | The title of the html page. Only for saving to html stream. |
| [AttachedFilesDirectory](#attachedfilesdirectory) | String | The directory that the attached files will be saved to. Only for saving to html stream. |
| [AttachedFilesUrlPrefix](#attachedfilesurlprefix) | String | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [DefaultFontName](#defaultfontname) | String | Specify the default font name for exporting html, the default font will be used when the font of style is not existing,  |
| [AddGenericFont](#addgenericfont) | boolean | Indicates whether to add a generic font to CSS font-family. The default value is true |
| [WorksheetScalable](#worksheetscalable) | boolean | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [IsExportComments](#isexportcomments) | boolean | Indicates if exporting comments when saving file to html, the default value is false. |
| [ExportCommentsType](#exportcommentstype) | int | Represents type of exporting comments to html files. The value of the property is PrintCommentsType integer constant. |
| [DisableDownlevelRevealedComments](#disabledownlevelrevealedcomments) | boolean | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [IsExpImageToTempDir](#isexpimagetotempdir) | boolean | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [ImageScalable](#imagescalable) | boolean | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. |
| [WidthScalable](#widthscalable) | boolean | Indicates whether exporting column width in unit of scale to html. The default value is false. |
| [ExportSingleTab](#exportsingletab) | boolean | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [ExportImagesAsBase64](#exportimagesasbase64) | boolean | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data |
| [ExportActiveWorksheetOnly](#exportactiveworksheetonly) | boolean | Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported t |
| [ExportPrintAreaOnly](#exportprintareaonly) | boolean | Indicates if only exporting the print area to html file. The default value is false. |
| [ExportArea](#exportarea) | CellArea | Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current ac |
| [ParseHtmlTagInCell](#parsehtmltagincell) | boolean | Indicates whether html tag(such as <div></div> ) in cell should be parsed as cell value or preserved as it is. The defau |
| [HtmlCrossStringType](#htmlcrossstringtype) | int | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. |
| [HiddenColDisplayType](#hiddencoldisplaytype) | int | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is  |
| [HiddenRowDisplayType](#hiddenrowdisplaytype) | int | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remo |
| [Encoding](#encoding) | Encoding | If not set,use Encoding.UTF8 as default enconding type. |
| [ExportObjectListener](#exportobjectlistener) | IExportObjectListener | Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use Ht |
| [FilePathProvider](#filepathprovider) | IFilePathProvider | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [ImageOptions](#imageoptions) | ImageOrPrintOptions | Get the ImageOrPrintOptions object before exporting |
| [SaveAsSingleFile](#saveassinglefile) | boolean | Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other re |
| [ShowAllSheets](#showallsheets) | boolean | Indicates whether showing all sheets when saving as a single html file. Only works when SaveAsSingleFile is True. |
| [ExportPageHeaders](#exportpageheaders) | boolean | Indicates whether exporting page headers. Only works when SaveAsSingleFile is True. |
| [ExportPageFooters](#exportpagefooters) | boolean | Indicates whether exporting page headers. Only works when SaveAsSingleFile is True. |
| [ExportHiddenWorksheet](#exporthiddenworksheet) | boolean | Indicating if exporting the hidden worksheet content.The default value is true. |
| [PresentationPreference](#presentationpreference) | boolean | Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful |
| [CellCssPrefix](#cellcssprefix) | String | Gets and sets the prefix of the css name,the default value is "". |
| [TableCssId](#tablecssid) | String | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which |
| [IsFullPathLink](#isfullpathlink) | boolean | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [ExportWorksheetCSSSeparately](#exportworksheetcssseparately) | boolean | Indicating whether export the worksheet css separately.The default value is false. |
| [ExportSimilarBorderStyle](#exportsimilarborderstyle) | boolean | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to |
| [MergeEmptyTdForcely](#mergeemptytdforcely) | boolean | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced s |
| [MergeEmptyTdType](#mergeemptytdtype) | int | The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. The value o |
| [ExportCellCoordinate](#exportcellcoordinate) | boolean | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If  |
| [ExportExtraHeadings](#exportextraheadings) | boolean | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value  |
| [ExportHeadings](#exportheadings) | boolean | Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete.  |
| [ExportRowColumnHeadings](#exportrowcolumnheadings) | boolean | Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false. |
| [ExportFormula](#exportformula) | boolean | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the outpu |
| [AddTooltipText](#addtooltiptext) | boolean | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [ExportGridLines](#exportgridlines) | boolean | Indicating whether exporting the gridlines.The default value is false. |
| [ExportBogusRowData](#exportbogusrowdata) | boolean | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file |
| [ExcludeUnusedStyles](#excludeunusedstyles) | boolean | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size  |
| [ExportDocumentProperties](#exportdocumentproperties) | boolean | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to |
| [ExportWorksheetProperties](#exportworksheetproperties) | boolean | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file t |
| [ExportWorkbookProperties](#exportworkbookproperties) | boolean | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to |
| [ExportFrameScriptsAndProperties](#exportframescriptsandproperties) | boolean | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the  |
| [ExportDataOptions](#exportdataoptions) | int | Indicating the rule of exporting html file data.The default value is All. The value of the property is HtmlExportDataOpt |
| [LinkTargetType](#linktargettype) | int | Indicating the type of target attribute in <a> link. The default value is HtmlLinkTargetType.Parent. The value of the pr |
| [IsIECompatible](#isiecompatible) | boolean | Indicating whether the output HTML is compatible with IE browser. The defalut value is false |
| [FormatDataIgnoreColumnWidth](#formatdataignorecolumnwidth) | boolean | Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column wid |
| [CalculateFormula](#calculateformula) | boolean | Indicates whether to calculate formulas before saving html file. The default value is false. |
| [IsJsBrowserCompatible](#isjsbrowsercompatible) | boolean | Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true. |
| [IsMobileCompatible](#ismobilecompatible) | boolean | Indicates whether the output HTML is compatible with mobile devices. The default value is false. |
| [CssStyles](#cssstyles) | String | Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. Example: CssStyles=" |
| [HideOverflowWrappedText](#hideoverflowwrappedtext) | boolean | Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false |
| [IsBorderCollapsed](#isbordercollapsed) | boolean | Indicates whether the table borders are collapsed. The default value is true. |
| [EncodeEntityAsCode](#encodeentityascode) | boolean |  |
| [OfficeMathOutputMode](#officemathoutputmode) | int | The value of the property is HtmlOfficeMathOutputType integer constant. |
| [CellNameAttribute](#cellnameattribute) | String |  |
| [DisableCss](#disablecss) | boolean |  |
| [EnableCssCustomProperties](#enablecsscustomproperties) | boolean |  |
| [HtmlVersion](#htmlversion) | int | The value of the property is HtmlVersion integer constant. |
| [SheetSet](#sheetset) | SheetSet |  |
| [LayoutMode](#layoutmode) | int | The value of the property is HtmlLayoutMode integer constant. |
| [EmbeddedFontType](#embeddedfonttype) | int | The value of the property is HtmlEmbeddedFontType integer constant. |
| [ExportNamedRangeAnchors](#exportnamedrangeanchors) | boolean |  |
| [DataBarRenderMode](#databarrendermode) | int | The value of the property is DataBarRenderMode integer constant. |
| [SpaceMode](#spacemode) | int | The value of the property is HtmlSpaceMode integer constant. |
| [SaveFormat](#saveformat) | int | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [ClearData](#cleardata) | boolean | Make the workbook empty after saving the file. |
| [CachedFileFolder](#cachedfilefolder) | String | The cached file folder is used to store some large data. |
| [ValidateMergedAreas](#validatemergedareas) | boolean | Indicates whether validate merged cells before saving the file. The default value is false. |
| [MergeAreas](#mergeareas) | boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [CreateDirectory](#createdirectory) | boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [SortNames](#sortnames) | boolean | Indicates whether sorting defined names before saving file. |
| [SortExternalNames](#sortexternalnames) | boolean | Indicates whether sorting external defined names before saving file. |
| [RefreshChartCache](#refreshchartcache) | boolean | Indicates whether refreshing chart cache data |
| [WarningCallback](#warningcallback) | IWarningCallback | Gets or sets warning callback. |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean |  |
| [UpdateSmartArt](#updatesmartart) | boolean | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [EncryptDocumentProperties](#encryptdocumentproperties) | boolean |  |

### HtmlSaveOptions() (1 of 2) {#constructor}

Creates options for saving html file.

---

### HtmlSaveOptions(saveFormat) (2 of 2) {#constructor-1}

Creates options for saving htm file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | A SaveFormat value. The file format. It should be one of following types: SaveFormat.HTML , SaveFormat.M_HTML , or SaveFormat.X_HTML , otherwise the saved format will be set as SaveFormat.HTML automatically. |

### HtmlSaveOptions.IgnoreInvisibleShapes property {#ignoreinvisibleshapes}

Indicate whether exporting those not visible shapes The default values is false.

**Type:** boolean

### HtmlSaveOptions.PageTitle property {#pagetitle}

The title of the html page. Only for saving to html stream.

**Type:** String

### HtmlSaveOptions.AttachedFilesDirectory property {#attachedfilesdirectory}

The directory that the attached files will be saved to. Only for saving to html stream.

**Type:** String

### HtmlSaveOptions.AttachedFilesUrlPrefix property {#attachedfilesurlprefix}

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

**Type:** String

### HtmlSaveOptions.DefaultFontName property {#defaultfontname}

Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

**Type:** String

### HtmlSaveOptions.AddGenericFont property {#addgenericfont}

Indicates whether to add a generic font to CSS font-family. The default value is true

**Type:** boolean

### HtmlSaveOptions.WorksheetScalable property {#worksheetscalable}

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

**Type:** boolean

### HtmlSaveOptions.IsExportComments property {#isexportcomments}

Indicates if exporting comments when saving file to html, the default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportCommentsType property {#exportcommentstype}

Represents type of exporting comments to html files. The value of the property is PrintCommentsType integer constant.

**Type:** int

### HtmlSaveOptions.DisableDownlevelRevealedComments property {#disabledownlevelrevealedcomments}

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

**Type:** boolean

### HtmlSaveOptions.IsExpImageToTempDir property {#isexpimagetotempdir}

Indicates whether exporting image files to temp directory. Only for saving to html stream.

**Type:** boolean

### HtmlSaveOptions.ImageScalable property {#imagescalable}

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

**Type:** boolean

### HtmlSaveOptions.WidthScalable property {#widthscalable}

Indicates whether exporting column width in unit of scale to html. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportSingleTab property {#exportsingletab}

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportImagesAsBase64 property {#exportimagesasbase64}

Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data is exported directly on the img elements and separate files are not created.

**Type:** boolean

### HtmlSaveOptions.ExportActiveWorksheetOnly property {#exportactiveworksheetonly}

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportPrintAreaOnly property {#exportprintareaonly}

Indicates if only exporting the print area to html file. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportArea property {#exportarea}

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

**Type:** CellArea

### HtmlSaveOptions.ParseHtmlTagInCell property {#parsehtmltagincell}

Indicates whether html tag(such as <div></div> ) in cell should be parsed as cell value or preserved as it is. The default value is true.

**Type:** boolean

### HtmlSaveOptions.HtmlCrossStringType property {#htmlcrossstringtype}

Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. The value of the property is HtmlCrossType integer constant.

**Type:** int

### HtmlSaveOptions.HiddenColDisplayType property {#hiddencoldisplaytype}

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" The value of the property is HtmlHiddenColDisplayType integer constant.

**Type:** int

### HtmlSaveOptions.HiddenRowDisplayType property {#hiddenrowdisplaytype}

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" The value of the property is HtmlHiddenRowDisplayType integer constant.

**Type:** int

### HtmlSaveOptions.Encoding property {#encoding}

If not set,use Encoding.UTF8 as default enconding type.

**Type:** Encoding

### HtmlSaveOptions.ExportObjectListener property {#exportobjectlistener}

Gets or sets the ExportObjectListener for exporting objects. NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.

**Type:** IExportObjectListener

### HtmlSaveOptions.FilePathProvider property {#filepathprovider}

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

**Type:** IFilePathProvider

### HtmlSaveOptions.ImageOptions property {#imageoptions}

Get the ImageOrPrintOptions object before exporting

**Type:** ImageOrPrintOptions

### HtmlSaveOptions.SaveAsSingleFile property {#saveassinglefile}

Indicates whether save the html as single file. The default value is false. If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

**Type:** boolean

### HtmlSaveOptions.ShowAllSheets property {#showallsheets}

Indicates whether showing all sheets when saving as a single html file. Only works when SaveAsSingleFile is True.

**Type:** boolean

### HtmlSaveOptions.ExportPageHeaders property {#exportpageheaders}

Indicates whether exporting page headers. Only works when SaveAsSingleFile is True.

**Type:** boolean

### HtmlSaveOptions.ExportPageFooters property {#exportpagefooters}

Indicates whether exporting page headers. Only works when SaveAsSingleFile is True.

**Type:** boolean

### HtmlSaveOptions.ExportHiddenWorksheet property {#exporthiddenworksheet}

Indicating if exporting the hidden worksheet content.The default value is true.

**Type:** boolean

### HtmlSaveOptions.PresentationPreference property {#presentationpreference}

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

**Type:** boolean

### HtmlSaveOptions.CellCssPrefix property {#cellcssprefix}

Gets and sets the prefix of the css name,the default value is "".

**Type:** String

### HtmlSaveOptions.TableCssId property {#tablecssid}

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

**Type:** String

### HtmlSaveOptions.IsFullPathLink property {#isfullpathlink}

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportWorksheetCSSSeparately property {#exportworksheetcssseparately}

Indicating whether export the worksheet css separately.The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportSimilarBorderStyle property {#exportsimilarborderstyle}

Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.

**Type:** boolean

### HtmlSaveOptions.MergeEmptyTdForcely property {#mergeemptytdforcely}

Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.MergeEmptyTdType property {#mergeemptytdtype}

The option to merge contiguous empty cells(empty td elements) The default value is MergeEmptyTdType.Default. The value of the property is MergeEmptyTdType integer constant.

**Type:** int

### HtmlSaveOptions.ExportCellCoordinate property {#exportcellcoordinate}

Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExportExtraHeadings property {#exportextraheadings}

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExportHeadings property {#exportheadings}

Indicates whether exports sheet's row and column headings when saving to HTML files. NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### HtmlSaveOptions.ExportRowColumnHeadings property {#exportrowcolumnheadings}

Indicates whether exports sheet's row and column headings when saving to HTML files. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportFormula property {#exportformula}

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.AddTooltipText property {#addtooltiptext}

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportGridLines property {#exportgridlines}

Indicating whether exporting the gridlines.The default value is false.

**Type:** boolean

### HtmlSaveOptions.ExportBogusRowData property {#exportbogusrowdata}

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExcludeUnusedStyles property {#excludeunusedstyles}

Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.

**Type:** boolean

### HtmlSaveOptions.ExportDocumentProperties property {#exportdocumentproperties}

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExportWorksheetProperties property {#exportworksheetproperties}

Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExportWorkbookProperties property {#exportworkbookproperties}

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExportFrameScriptsAndProperties property {#exportframescriptsandproperties}

Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

**Type:** boolean

### HtmlSaveOptions.ExportDataOptions property {#exportdataoptions}

Indicating the rule of exporting html file data.The default value is All. The value of the property is HtmlExportDataOptions integer constant.

**Type:** int

### HtmlSaveOptions.LinkTargetType property {#linktargettype}

Indicating the type of target attribute in <a> link. The default value is HtmlLinkTargetType.Parent. The value of the property is HtmlLinkTargetType integer constant.

**Type:** int

### HtmlSaveOptions.IsIECompatible property {#isiecompatible}

Indicating whether the output HTML is compatible with IE browser. The defalut value is false

**Type:** boolean

### HtmlSaveOptions.FormatDataIgnoreColumnWidth property {#formatdataignorecolumnwidth}

Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.

**Type:** boolean

### HtmlSaveOptions.CalculateFormula property {#calculateformula}

Indicates whether to calculate formulas before saving html file. The default value is false.

**Type:** boolean

### HtmlSaveOptions.IsJsBrowserCompatible property {#isjsbrowsercompatible}

Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.

**Type:** boolean

### HtmlSaveOptions.IsMobileCompatible property {#ismobilecompatible}

Indicates whether the output HTML is compatible with mobile devices. The default value is false.

**Type:** boolean

### HtmlSaveOptions.CssStyles property {#cssstyles}

Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True. Example: CssStyles="body { padding: 5px }";

**Type:** String

### HtmlSaveOptions.HideOverflowWrappedText property {#hideoverflowwrappedtext}

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

**Type:** boolean

### HtmlSaveOptions.IsBorderCollapsed property {#isbordercollapsed}

Indicates whether the table borders are collapsed. The default value is true.

**Type:** boolean

### HtmlSaveOptions.EncodeEntityAsCode property {#encodeentityascode}

**Type:** boolean

### HtmlSaveOptions.OfficeMathOutputMode property {#officemathoutputmode}

The value of the property is HtmlOfficeMathOutputType integer constant.

**Type:** int

### HtmlSaveOptions.CellNameAttribute property {#cellnameattribute}

**Type:** String

### HtmlSaveOptions.DisableCss property {#disablecss}

**Type:** boolean

### HtmlSaveOptions.EnableCssCustomProperties property {#enablecsscustomproperties}

**Type:** boolean

### HtmlSaveOptions.HtmlVersion property {#htmlversion}

The value of the property is HtmlVersion integer constant.

**Type:** int

### HtmlSaveOptions.SheetSet property {#sheetset}

**Type:** SheetSet

### HtmlSaveOptions.LayoutMode property {#layoutmode}

The value of the property is HtmlLayoutMode integer constant.

**Type:** int

### HtmlSaveOptions.EmbeddedFontType property {#embeddedfonttype}

The value of the property is HtmlEmbeddedFontType integer constant.

**Type:** int

### HtmlSaveOptions.ExportNamedRangeAnchors property {#exportnamedrangeanchors}

**Type:** boolean

### HtmlSaveOptions.DataBarRenderMode property {#databarrendermode}

The value of the property is DataBarRenderMode integer constant.

**Type:** int

### HtmlSaveOptions.SpaceMode property {#spacemode}

The value of the property is HtmlSpaceMode integer constant.

**Type:** int

### HtmlSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** int

### HtmlSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### HtmlSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### HtmlSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### HtmlSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### HtmlSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### HtmlSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### HtmlSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### HtmlSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### HtmlSaveOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### HtmlSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### HtmlSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### HtmlSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
