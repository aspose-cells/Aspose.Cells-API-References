##PdfSaveOptions Class
'PdfSaveOptions class. Encapsulates the object that represents pdfsaveoptions in Go.'
## PdfSaveOptions class
Represents the options for saving pdf file.
```go
type PdfSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPdfSaveOptions](./newpdfsaveoptions/) | Creates the options for saving pdf file. |
|[NewPdfSaveOptions_PaginatedSaveOptions](./newpdfsaveoptions_paginatedsaveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetEmbedStandardWindowsFonts](./getembedstandardwindowsfonts/) | True to embed true type fonts.Affects only ASCII characters 32-127.Fonts for character codes greater than 127 are always embedded.Fonts are always embedded for PDF/A-1a, PDF/A-1b standard.Default is true. |
|[SetEmbedStandardWindowsFonts](./setembedstandardwindowsfonts/) | True to embed true type fonts.Affects only ASCII characters 32-127.Fonts for character codes greater than 127 are always embedded.Fonts are always embedded for PDF/A-1a, PDF/A-1b standard.Default is true. |
|[GetBookmark](./getbookmark/) | Gets and sets the PdfBookmarkEntry</see> object. |
|[SetBookmark](./setbookmark/) | Gets and sets the PdfBookmarkEntry</see> object. |
|[GetCompliance](./getcompliance/) | Gets or sets the PDF standards compliance level for output documents. |
|[SetCompliance](./setcompliance/) | Gets or sets the PDF standards compliance level for output documents. |
|[GetSecurityOptions](./getsecurityoptions/) | Set this options, when security is need in xls2pdf result. |
|[SetSecurityOptions](./setsecurityoptions/) | Set this options, when security is need in xls2pdf result. |
|[GetCalculateFormula](./getcalculateformula/) | Indicates whether to calculate formulas before saving pdf file. |
|[SetCalculateFormula](./setcalculateformula/) | Indicates whether to calculate formulas before saving pdf file. |
|[GetPdfCompression](./getpdfcompression/) | Indicate the compression algorithm |
|[SetPdfCompression](./setpdfcompression/) | Indicate the compression algorithm |
|[SetImageResample](./setimageresample/) | Sets desired PPI(pixels per inch) of resample images and jpeg quality.All images will be converted to JPEG with the specified quality setting,and images that are greater than the specified PPI (pixels per inch) will be resampled. |
|[GetCreatedTime](./getcreatedtime/) | Gets and sets the time of generating the pdf document. |
|[SetCreatedTime](./setcreatedtime/) | Gets and sets the time of generating the pdf document. |
|[GetProducer](./getproducer/) | Gets and sets producer of generated pdf document. |
|[SetProducer](./setproducer/) | Gets and sets producer of generated pdf document. |
|[GetOptimizationType](./getoptimizationtype/) | Gets and sets pdf optimization type. |
|[SetOptimizationType](./setoptimizationtype/) | Gets and sets pdf optimization type. |
|[GetCustomPropertiesExport](./getcustompropertiesexport/) | Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None. |
|[SetCustomPropertiesExport](./setcustompropertiesexport/) | Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None. |
|[GetExportDocumentStructure](./getexportdocumentstructure/) | Indicates whether to export document structure. |
|[SetExportDocumentStructure](./setexportdocumentstructure/) | Indicates whether to export document structure. |
|[GetDisplayDocTitle](./getdisplaydoctitle/) | Indicates whether the window's title bar should display the document title. |
|[SetDisplayDocTitle](./setdisplaydoctitle/) | Indicates whether the window's title bar should display the document title. |
|[GetFontEncoding](./getfontencoding/) | Gets or sets embedded font encoding in pdf. |
|[SetFontEncoding](./setfontencoding/) | Gets or sets embedded font encoding in pdf. |
|[GetWatermark](./getwatermark/) | Gets or sets watermark to output. |
|[SetWatermark](./setwatermark/) | Gets or sets watermark to output. |
|[GetEmbedAttachments](./getembedattachments/) | Indicates whether to embed attachment for Ole objects in Excel. |
|[SetEmbedAttachments](./setembedattachments/) | Indicates whether to embed attachment for Ole objects in Excel. |
|[GetDefaultFont](./getdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
|[SetDefaultFont](./setdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
|[GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first. |
|[SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first. |
|[SetCheckFontCompatibility](./setcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. |
|[GetCheckFontCompatibility](./getcheckfontcompatibility/) | Indicates whether to check font compatibility for every character in text. |
|[SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
|[IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
|[GetOnePagePerSheet](./getonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result.The paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. |
|[SetOnePagePerSheet](./setonepagepersheet/) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result.The paper size of pagesetup will be invalid, and the other settings of pagesetupwill still take effect. |
|[GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result.The width of paper size of pagesetup will be ignored, and the other settings of pagesetupwill still take effect. |
|[SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result.The width of paper size of pagesetup will be ignored, and the other settings of pagesetupwill still take effect. |
|[GetIgnoreError](./getignoreerror/) | Indicates if you need to hide the error while rendering.The error can be error in shape, image, chart rendering, etc. |
|[SetIgnoreError](./setignoreerror/) | Indicates if you need to hide the error while rendering.The error can be error in shape, image, chart rendering, etc. |
|[GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
|[SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indicates whether to output a blank page when there is nothing to print. |
|[SetPageIndex](./setpageindex/) | Gets or sets the 0-based index of the first page to save. |
|[GetPageIndex](./getpageindex/) | Gets or sets the 0-based index of the first page to save. |
|[SetPageCount](./setpagecount/) | Gets or sets the number of pages to save. |
|[GetPageCount](./getpagecount/) | Gets or sets the number of pages to save. |
|[GetPrintingPageType](./getprintingpagetype/) | Indicates which pages will not be printed. |
|[SetPrintingPageType](./setprintingpagetype/) | Indicates which pages will not be printed. |
|[GetGridlineType](./getgridlinetype/) | Gets or sets gridline type. |
|[SetGridlineType](./setgridlinetype/) | Gets or sets gridline type. |
|[GetGridlineColor](./getgridlinecolor/) | Gets or sets gridline color. |
|[SetGridlineColor](./setgridlinecolor/) | Gets or sets gridline color. |
|[GetTextCrossType](./gettextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
|[SetTextCrossType](./settextcrosstype/) | Gets or sets displaying text type when the text width is larger than cell width. |
|[GetDefaultEditLanguage](./getdefaulteditlanguage/) | Gets or sets default edit language. |
|[SetDefaultEditLanguage](./setdefaulteditlanguage/) | Gets or sets default edit language. |
|[GetSheetSet](./getsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
|[SetSheetSet](./setsheetset/) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible. |
|[GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
|[SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implements this interface to get DrawObject and Bound when rendering. |
|[GetEmfRenderSetting](./getemfrendersetting/) | Setting for rendering Emf metafile. |
|[SetEmfRenderSetting](./setemfrendersetting/) | Setting for rendering Emf metafile. |
|[GetCustomRenderSettings](./getcustomrendersettings/) | Gets or sets custom settings during rendering. |
|[SetCustomRenderSettings](./setcustomrendersettings/) | Gets or sets custom settings during rendering. |
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
