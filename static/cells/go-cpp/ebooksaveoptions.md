##EbookSaveOptions Class
'EbookSaveOptions class. Encapsulates the object that represents ebooksaveoptions in Go.'
## EbookSaveOptions class
Represents the options for saving ebook file.
```go
type EbookSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewEbookSaveOptions](./newebooksaveoptions/) | Creates options for saving ebook file. |
|[NewEbookSaveOptions_SaveFormat](./newebooksaveoptions_saveformat/) | Creates options for saving ebook file. |
|[NewEbookSaveOptions_HtmlSaveOptions](./newebooksaveoptions_htmlsaveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes |
|[SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Indicate whether exporting those not visible shapes |
|[GetPageTitle](./getpagetitle/) | The title of the html page.Only for saving to html stream. |
|[SetPageTitle](./setpagetitle/) | The title of the html page.Only for saving to html stream. |
|[GetAttachedFilesDirectory](./getattachedfilesdirectory/) | The directory that the attached files will be saved to.Only for saving to html stream. |
|[SetAttachedFilesDirectory](./setattachedfilesdirectory/) | The directory that the attached files will be saved to.Only for saving to html stream. |
|[GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file.Only for saving to html stream. |
|[SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | Specify the Url prefix of attached files such as image in the html file.Only for saving to html stream. |
|[GetDefaultFontName](./getdefaultfontname/) | Specify the default font name for exporting html, the default font will be used  when the font of style is not existing,If this property is null, Aspose.Cells will use universal font which have the same family with the original font,the default value is null. |
|[SetDefaultFontName](./setdefaultfontname/) | Specify the default font name for exporting html, the default font will be used  when the font of style is not existing,If this property is null, Aspose.Cells will use universal font which have the same family with the original font,the default value is null. |
|[GetAddGenericFont](./getaddgenericfont/) | Indicates whether to add a generic font to CSS font-family.The default value is true |
|[SetAddGenericFont](./setaddgenericfont/) | Indicates whether to add a generic font to CSS font-family.The default value is true |
|[GetWorksheetScalable](./getworksheetscalable/) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
|[SetWorksheetScalable](./setworksheetscalable/) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
|[IsExportComments](./isexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
|[SetIsExportComments](./setisexportcomments/) | Indicates if exporting comments when saving file to html, the default value is false. |
|[GetExportCommentsType](./getexportcommentstype/) | Represents type of exporting comments to html files. |
|[SetExportCommentsType](./setexportcommentstype/) | Represents type of exporting comments to html files. |
|[GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
|[SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
|[IsExpImageToTempDir](./isexpimagetotempdir/) | Indicates whether exporting image files to temp directory.Only for saving to html stream. |
|[SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Indicates whether exporting image files to temp directory.Only for saving to html stream. |
|[GetImageScalable](./getimagescalable/) | Indicates whether using scalable unit to describe the image widthwhen using scalable unit to describe the column width.The default value is true. |
|[SetImageScalable](./setimagescalable/) | Indicates whether using scalable unit to describe the image widthwhen using scalable unit to describe the column width.The default value is true. |
|[GetWidthScalable](./getwidthscalable/) | Indicates whether exporting column width in unit of scale to html.The default value is false. |
|[SetWidthScalable](./setwidthscalable/) | Indicates whether exporting column width in unit of scale to html.The default value is false. |
|[GetExportSingleTab](./getexportsingletab/) | Indicates whether exporting the single tab when the file only has one worksheet.The default value is false. |
|[SetExportSingleTab](./setexportsingletab/) | Indicates whether exporting the single tab when the file only has one worksheet.The default value is false. |
|[GetExportImagesAsBase64](./getexportimagesasbase64/) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
|[SetExportImagesAsBase64](./setexportimagesasbase64/) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
|[GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Indicates if only exporting the active worksheet to html file.If true then only the active worksheet will be exported to html file;If false then the whole workbook will be exported to html file.The default value is false. |
|[SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Indicates if only exporting the active worksheet to html file.If true then only the active worksheet will be exported to html file;If false then the whole workbook will be exported to html file.The default value is false. |
|[GetExportPrintAreaOnly](./getexportprintareaonly/) | Indicates if only exporting the print area to html file. The default value is false. |
|[SetExportPrintAreaOnly](./setexportprintareaonly/) | Indicates if only exporting the print area to html file. The default value is false. |
|[GetExportArea](./getexportarea/) | Gets or Sets the exporting CellArea of current active Worksheet.If you set this attribute, the print area of current active Worksheet will be omitted.Only the specified area will be exported when saving the file to html. |
|[SetExportArea](./setexportarea/) | Gets or Sets the exporting CellArea of current active Worksheet.If you set this attribute, the print area of current active Worksheet will be omitted.Only the specified area will be exported when saving the file to html. |
|[GetParseHtmlTagInCell](./getparsehtmltagincell/) | Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is.The default value is true. |
|[SetParseHtmlTagInCell](./setparsehtmltagincell/) | Indicates whether html tag(such as <c>&lt;div&gt;&lt;/div&gt;</c>) in cell should be parsed as cell value or preserved as it is.The default value is true. |
|[GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel.But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
|[SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel.But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
|[GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Hidden column(the width of this column is 0) in excel,before save this into html format,if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output,if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
|[SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Hidden column(the width of this column is 0) in excel,before save this into html format,if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output,if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
|[GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Hidden row(the height of this row is 0) in excel,before save this into html format,if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output,if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
|[SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Hidden row(the height of this row is 0) in excel,before save this into html format,if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output,if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
|[GetEncoding](./getencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
|[SetEncoding](./setencoding/) | If not set,use Encoding.UTF8 as default enconding type. |
|[GetImageOptions](./getimageoptions/) | Get the ImageOrPrintOptions object before exporting |
|[GetSaveAsSingleFile](./getsaveassinglefile/) | Indicates whether save the html as single file.The default value is false. |
|[SetSaveAsSingleFile](./setsaveassinglefile/) | Indicates whether save the html as single file.The default value is false. |
|[GetShowAllSheets](./getshowallsheets/) | Indicates whether showing all sheets when saving  as a single html file. |
|[SetShowAllSheets](./setshowallsheets/) | Indicates whether showing all sheets when saving  as a single html file. |
|[GetExportPageHeaders](./getexportpageheaders/) | Indicates whether exporting page headers. |
|[SetExportPageHeaders](./setexportpageheaders/) | Indicates whether exporting page headers. |
|[GetExportPageFooters](./getexportpagefooters/) | Indicates whether exporting page headers. |
|[SetExportPageFooters](./setexportpagefooters/) | Indicates whether exporting page headers. |
|[GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Indicating if exporting the hidden worksheet content.The default value is true. |
|[SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Indicating if exporting the hidden worksheet content.The default value is true. |
|[GetPresentationPreference](./getpresentationpreference/) | Indicating if html or mht file is presentation preference.The default value is false.if you want to get more beautiful presentation,please set the value to true. |
|[SetPresentationPreference](./setpresentationpreference/) | Indicating if html or mht file is presentation preference.The default value is false.if you want to get more beautiful presentation,please set the value to true. |
|[GetCellCssPrefix](./getcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
|[SetCellCssPrefix](./setcellcssprefix/) | Gets and sets the prefix of the css name,the default value is "". |
|[GetTableCssId](./gettablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table elementwhich has the specific TableCssId attribute. The default value is "". |
|[SetTableCssId](./settablecssid/) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table elementwhich has the specific TableCssId attribute. The default value is "". |
|[IsFullPathLink](./isfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm.The default value is false. |
|[SetIsFullPathLink](./setisfullpathlink/) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm.The default value is false. |
|[GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Indicating whether export the worksheet css separately.The default value is false. |
|[SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Indicating whether export the worksheet css separately.The default value is false. |
|[GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Indicating whether exporting the similar border style when the border style is not supported by browsers.If you want to import the html or mht file to excel, please keep the default value.The default value is false. |
|[SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Indicating whether exporting the similar border style when the border style is not supported by browsers.If you want to import the html or mht file to excel, please keep the default value.The default value is false. |
|[GetMergeEmptyTdType](./getmergeemptytdtype/) | The option to merge contiguous empty cells(empty td elements)The default value is MergeEmptyTdType.Default. |
|[SetMergeEmptyTdType](./setmergeemptytdtype/) | The option to merge contiguous empty cells(empty td elements)The default value is MergeEmptyTdType.Default. |
|[GetExportCellCoordinate](./getexportcellcoordinate/) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false.If you want to import the output html to excel, please keep the default value. |
|[SetExportCellCoordinate](./setexportcellcoordinate/) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false.If you want to import the output html to excel, please keep the default value. |
|[GetExportExtraHeadings](./getexportextraheadings/) | Indicates whether exporting extra headings when the length of text is longer than max display column.The default value is false. If you want to import the html file to excel, please keep the default value. |
|[SetExportExtraHeadings](./setexportextraheadings/) | Indicates whether exporting extra headings when the length of text is longer than max display column.The default value is false. If you want to import the html file to excel, please keep the default value. |
|[GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
|[SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
|[GetExportFormula](./getexportformula/) | Indicates whether exporting formula when saving file to html. The default value is true.If you want to import the output html to excel, please keep the default value. |
|[SetExportFormula](./setexportformula/) | Indicates whether exporting formula when saving file to html. The default value is true.If you want to import the output html to excel, please keep the default value. |
|[GetAddTooltipText](./getaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed.The default value is false. |
|[SetAddTooltipText](./setaddtooltiptext/) | Indicates whether adding tooltip text when the data can't be fully displayed.The default value is false. |
|[GetExportGridLines](./getexportgridlines/) | Indicating whether exporting the gridlines.The default value is false. |
|[SetExportGridLines](./setexportgridlines/) | Indicating whether exporting the gridlines.The default value is false. |
|[GetExportBogusRowData](./getexportbogusrowdata/) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht fileto excel, please keep the default value. |
|[SetExportBogusRowData](./setexportbogusrowdata/) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht fileto excel, please keep the default value. |
|[GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Indicating whether excludes unused styles.For the generated html files, excluding unused styles can make the file size smallerwithout affecting the visual effects. So the default value of this property is true.If user needs to keep all styles in the workbook for the generated html(such as the scenario that userneeds to restore the workbook from the generated html later), please set this property as false. |
|[SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Indicating whether excludes unused styles.For the generated html files, excluding unused styles can make the file size smallerwithout affecting the visual effects. So the default value of this property is true.If user needs to keep all styles in the workbook for the generated html(such as the scenario that userneeds to restore the workbook from the generated html later), please set this property as false. |
|[GetExportDocumentProperties](./getexportdocumentproperties/) | Indicating whether exporting document properties.The default value is true.If you want to importthe html or mht file to excel, please keep the default value. |
|[SetExportDocumentProperties](./setexportdocumentproperties/) | Indicating whether exporting document properties.The default value is true.If you want to importthe html or mht file to excel, please keep the default value. |
|[GetExportWorksheetProperties](./getexportworksheetproperties/) | Indicating whether exporting worksheet properties.The default value is true.If you want to importthe html or mht file to excel, please keep the default value. |
|[SetExportWorksheetProperties](./setexportworksheetproperties/) | Indicating whether exporting worksheet properties.The default value is true.If you want to importthe html or mht file to excel, please keep the default value. |
|[GetExportWorkbookProperties](./getexportworkbookproperties/) | Indicating whether exporting workbook properties.The default value is true.If you want to importthe html or mht file to excel, please keep the default value. |
|[SetExportWorkbookProperties](./setexportworkbookproperties/) | Indicating whether exporting workbook properties.The default value is true.If you want to importthe html or mht file to excel, please keep the default value. |
|[GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht fileto excel, please keep the default value. |
|[SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht fileto excel, please keep the default value. |
|[GetExportDataOptions](./getexportdataoptions/) | Indicating the rule of exporting html file data.The default value is All. |
|[SetExportDataOptions](./setexportdataoptions/) | Indicating the rule of exporting html file data.The default value is All. |
|[GetLinkTargetType](./getlinktargettype/) | Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
|[SetLinkTargetType](./setlinktargettype/) | Indicating the type of target attribute in <c>&lt;a&gt;</c> link. The default value is HtmlLinkTargetType.Parent. |
|[IsIECompatible](./isiecompatible/) | Indicating whether the output HTML is compatible with IE browser.The defalut value is false |
|[SetIsIECompatible](./setisiecompatible/) | Indicating whether the output HTML is compatible with IE browser.The defalut value is false |
|[GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Indicating whether show the whole formatted data of cell when overflowing the column.If true then ignore the column width and the whole data of cell will be exported.If false then the data will be exported same as Excel.The default value is false. |
|[SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Indicating whether show the whole formatted data of cell when overflowing the column.If true then ignore the column width and the whole data of cell will be exported.If false then the data will be exported same as Excel.The default value is false. |
|[GetCalculateFormula](./getcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
|[SetCalculateFormula](./setcalculateformula/) | Indicates whether to calculate formulas before saving html file. |
|[IsJsBrowserCompatible](./isjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript.The default value is true. |
|[SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript.The default value is true. |
|[IsMobileCompatible](./ismobilecompatible/) | Indicates whether the output HTML is compatible with mobile devices.The default value is false. |
|[SetIsMobileCompatible](./setismobilecompatible/) | Indicates whether the output HTML is compatible with mobile devices.The default value is false. |
|[GetCssStyles](./getcssstyles/) | Gets or sets the additional css styles for the formatter.Only works when SaveAsSingleFile is True. |
|[SetCssStyles](./setcssstyles/) | Gets or sets the additional css styles for the formatter.Only works when SaveAsSingleFile is True. |
|[GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Indicates whether to hide overflow text when the cell format is set to wrap text.The default value is false |
|[SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Indicates whether to hide overflow text when the cell format is set to wrap text.The default value is false |
|[IsBorderCollapsed](./isbordercollapsed/) | Indicates whether the table borders are collapsed.The default value is true. |
|[SetIsBorderCollapsed](./setisbordercollapsed/) | Indicates whether the table borders are collapsed.The default value is true. |
|[GetEncodeEntityAsCode](./getencodeentityascode/) | Indicates whether the html character entities are replaced with decimal code.(e.g. "&amp;nbsp;" is replaced with "&amp;#160;").The default value is false. |
|[SetEncodeEntityAsCode](./setencodeentityascode/) | Indicates whether the html character entities are replaced with decimal code.(e.g. "&amp;nbsp;" is replaced with "&amp;#160;").The default value is false. |
|[GetOfficeMathOutputMode](./getofficemathoutputmode/) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
|[SetOfficeMathOutputMode](./setofficemathoutputmode/) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
|[GetCellNameAttribute](./getcellnameattribute/) | Specifies the attribute that indicates the CellName to be written.(e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;).The default value is null. |
|[SetCellNameAttribute](./setcellnameattribute/) | Specifies the attribute that indicates the CellName to be written.(e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;).The default value is null. |
|[GetDisableCss](./getdisablecss/) | Indicates whether only inline styles are applied, without relying on CSS.The default value is false. |
|[SetDisableCss](./setdisablecss/) | Indicates whether only inline styles are applied, without relying on CSS.The default value is false. |
|[GetEnableCssCustomProperties](./getenablecsscustomproperties/) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved.The default value is false. |
|[SetEnableCssCustomProperties](./setenablecsscustomproperties/) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved.The default value is false. |
|[GetHtmlVersion](./gethtmlversion/) | Specifies version of HTML standard that should be used when saving the HTML format.Default value is HtmlVersion.Default. |
|[SetHtmlVersion](./sethtmlversion/) | Specifies version of HTML standard that should be used when saving the HTML format.Default value is HtmlVersion.Default. |
|[GetSheetSet](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
|[SetSheetSet](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
|[GetEmbeddedFontType](./getembeddedfonttype/) | Gets or sets the type of font that embedded in html.Default value is HtmlEmbeddedFontType.None which indicates that it will not embed font in html. |
|[SetEmbeddedFontType](./setembeddedfonttype/) | Gets or sets the type of font that embedded in html.Default value is HtmlEmbeddedFontType.None which indicates that it will not embed font in html. |
|[GetSaveFormat](./getsaveformat/) | Gets the save file format. |
|[GetClearData](./getcleardata/) | Make the workbook empty after saving the file. |
|[SetClearData](./setcleardata/) | Make the workbook empty after saving the file. |
|[GetCachedFileFolder](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
|[SetCachedFileFolder](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
|[GetValidateMergedAreas](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
|[SetValidateMergedAreas](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
|[GetMergeAreas](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
|[SetMergeAreas](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
|[GetCreateDirectory](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
|[SetCreateDirectory](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
|[GetSortNames](./getsortnames/) | Indicates whether sorting defined names before saving file. |
|[SetSortNames](./setsortnames/) | Indicates whether sorting defined names before saving file. |
|[GetSortExternalNames](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
|[SetSortExternalNames](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
|[GetRefreshChartCache](./getrefreshchartcache/) | Indicates whether refreshing chart cache data |
|[SetRefreshChartCache](./setrefreshchartcache/) | Indicates whether refreshing chart cache data |
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
|[GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
|[SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
|[GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
|[SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
