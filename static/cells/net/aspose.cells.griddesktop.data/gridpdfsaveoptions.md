##Class GridPdfSaveOptions
Aspose.Cells.GridDesktop.Data.GridPdfSaveOptions class. Represents the options for saving pdf file
## GridPdfSaveOptions class
Represents the options for saving pdf file.
```csharp
public class GridPdfSaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [GridPdfSaveOptions](gridpdfsaveoptions/)() | The construct of GridSaveOptions |
## Properties
| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cachedfilefolder/) { get; set; } | The cached file folder is used to store some large data. |
| [CalculateFormula](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/calculateformula/) { get; set; } | Indicates whether to calculate formulas before saving pdf file. |
| [ClearData](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file. |
| [Compliance](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/compliance/) { get; set; } | Workbook converts to pdf will according to PdfCompliance in this property. |
| [CreateDirectory](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [CreatedTime](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdtime/) { get; set; } | Gets and sets the time of generating the pdf document. |
| [CustomPropertiesExport](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/custompropertiesexport/) { get; set; } | Gets or sets a value determining the way are exported to PDF file. Default value is None. |
| [DisplayDocTitle](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/displaydoctitle/) { get; set; } | Indicates whether the window's title bar should display the document title. |
| [EmbedStandardWindowsFonts](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [EmfRenderSetting](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/emfrendersetting/) { get; set; } | Setting for rendering Emf metafile. |
| [ExportDocumentStructure](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/exportdocumentstructure/) { get; set; } | Indicates whether to export document structure. |
| [FontEncoding](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/fontencoding/) { get; set; } | Gets or sets embedded font encoding in pdf. |
| [MergeAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [OptimizationType](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/optimizationtype/) { get; set; } | Gets and sets pdf optimization type. |
| [PdfCompression](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/pdfcompression/) { get; set; } | Indicate the compression algorithm |
| [Producer](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/producer/) { get; set; } | Gets and sets producer of generated pdf document. |
| [RefreshChartCache](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data |
| [SortExternalNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file. |
| [SortNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file. |
| [UpdateSmartArt](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false. |
| [ValidateMergedAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file. |
## Methods
| Name | Description |
| --- | --- |
| [SetImageResample](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/)(int, int) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled. |
### See Also
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)
