##Class PdfSaveOptions
Aspose.Cells.PdfSaveOptions class. Represents the options for saving pdf file
## PdfSaveOptions class
Represents the options for saving pdf file.
```csharp
public class PdfSaveOptions : PaginatedSaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Creates the options for saving pdf file. |
## Properties
| Name | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark/) { get; set; } | Gets and sets the [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry/) object. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula/) { get; set; } | Indicates whether to calculate formulas before saving pdf file. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indicates whether to check font compatibility for every character in text.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance/) { get; set; } | Gets or sets the PDF standards compliance level for output documents. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime/) { get; set; } | Gets and sets the time of generating the pdf document. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport/) { get; set; } | Gets or sets a value determining the way [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) are exported to PDF file. Default value is None. |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Gets or sets custom settings during rendering.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Gets or sets default edit language.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle/) { get; set; } | Indicates whether the window's title bar should display the document title. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implements this interface to get DrawObject and Bound when rendering.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedAttachments](../../aspose.cells/pdfsaveoptions/embedattachments/) { get; set; } | Indicates whether to embed attachment for Ole objects in Excel. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Setting for rendering Emf metafile.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure/) { get; set; } | Indicates whether to export document structure. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding/) { get; set; } | Gets or sets embedded font encoding in pdf. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Gets or sets gridline color.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Gets or sets gridline type.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ImageType](../../aspose.cells/pdfsaveoptions/imagetype/) { get; set; } | (**Obsolete.**) Represents the image type when converting the chart and shape . |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indicates whether to only substitute the font of character when the cell font is not compatibility for it.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype/) { get; set; } | Gets and sets pdf optimization type. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indicates whether to output a blank page when there is nothing to print.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Gets or sets the number of pages to save.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Gets or sets the 0-based index of the first page to save.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Control/Indicate progress of page saving process.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression/) { get; set; } | Indicate the compression algorithm |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indicates which pages will not be printed.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Producer](../../aspose.cells/pdfsaveoptions/producer/) { get; set; } | Gets and sets producer of generated pdf document. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions/) { get; set; } | Set this options, when security is need in xls2pdf result. |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Gets or sets displaying text type when the text width is larger than cell width.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [Watermark](../../aspose.cells/pdfsaveoptions/watermark/) { get; set; } | Gets or sets watermark to output. |
## Methods
| Name | Description |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample/)(int, int) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Rendering.PdfSecurity;
using System;
using System.Drawing;
public class PdfSaveOptionsDemo
{
public static void PdfSaveOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Save Options Example");
// Create an instance of PdfSaveOptions
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set various properties
pdfSaveOptions.EmbedStandardWindowsFonts = true;
pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
pdfSaveOptions.CalculateFormula = true;
pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
pdfSaveOptions.CreatedTime = DateTime.Now;
pdfSaveOptions.Producer = "Aspose.Cells";
pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
pdfSaveOptions.ExportDocumentStructure = true;
pdfSaveOptions.DisplayDocTitle = true;
pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
pdfSaveOptions.EmbedAttachments = true;
pdfSaveOptions.DefaultFont = "Arial";
pdfSaveOptions.CheckWorkbookDefaultFont = true;
pdfSaveOptions.CheckFontCompatibility = true;
pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
pdfSaveOptions.OnePagePerSheet = true;
pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
pdfSaveOptions.IgnoreError = true;
pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
pdfSaveOptions.PageIndex = 0;
pdfSaveOptions.PageCount = 1;
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
pdfSaveOptions.GridlineType = GridlineType.Dotted;
pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
pdfSaveOptions.SheetSet = SheetSet.Visible;
pdfSaveOptions.ClearData = true;
pdfSaveOptions.CachedFileFolder = "C:\\Temp";
pdfSaveOptions.ValidateMergedAreas = true;
pdfSaveOptions.MergeAreas = true;
pdfSaveOptions.SortNames = true;
pdfSaveOptions.SortExternalNames = true;
pdfSaveOptions.RefreshChartCache = true;
// Set security options
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
{
OwnerPassword = "OwnerPassword",
UserPassword = "UserPassword",
PrintPermission = true,
FullQualityPrintPermission = true
};
pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
// Set watermark
RenderingFont font = new RenderingFont("Calibri", 68)
{
Italic = true,
Bold = true,
Color = Color.Blue
};
RenderingWatermark watermark = new RenderingWatermark("Watermark", font)
{
HAlignment = TextAlignmentType.Center,
VAlignment = TextAlignmentType.Center,
Rotation = 30,
Opacity = 0.6f,
ScaleToPagePercent = 50
};
pdfSaveOptions.Watermark = watermark;
// Save the workbook as a PDF file
workbook.Save("PdfSaveOptionsExample.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
