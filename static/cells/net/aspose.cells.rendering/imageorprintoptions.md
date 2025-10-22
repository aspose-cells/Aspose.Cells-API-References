##Class ImageOrPrintOptions
Aspose.Cells.Rendering.ImageOrPrintOptions class. Allows to specify options when rendering worksheet to images printing worksheet or rendering chart to image
## ImageOrPrintOptions class
Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.
```csharp
public class ImageOrPrintOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Ctor. |
## Properties
| Name | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indicate the chart imagetype when converting. default value: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Client can special output to printer when print each page using this EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Client can control page setting of printer when print each page using this EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Gets or sets custom settings during rendering. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Gets or sets default edit language. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implements this interface to get DrawObject and Bound when rendering. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Setting for rendering Emf metafiles in source file. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Gets or sets gridline colr. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Gets or sets gridline type. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Gets or sets the format of the generated images. default value: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indicates whether to optimize the output elements. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | If this property is true , one Area will be output, and no scale will take effect. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indicates whether to output a blank page when there is nothing to print. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Gets or sets the number of pages to save. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Gets or sets the 0-based index of the first page to save. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Control/Indicate progress of page saving process. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Gets or sets the pixel format for the generated images. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indicates which pages will not be printed. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. The default value is 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Gets or sets the output file format type Support Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Specifies whether smoothing (antialiasing) is applied to lines and curves and the edges of filled areas. The default value is SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) if this property is true, the generated svg will fit to view port. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Gets or sets displaying text type when the text width is larger than cell width. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Gets or sets method used while converting images to 1 bpp format when [`ImageType`](./imagetype/) is Tiff and [`TiffCompression`](./tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Gets or sets bit depth to apply only when saving pages to the `Tiff` format. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Gets or sets the type of compression to apply only when saving pages to the `Tiff` format. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indicates if the background of generated image should be transparent. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Gets or sets warning callback. |
## Methods
| Name | Description |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Sets desired width and height of image. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Sets desired width and height of image. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class RenderingClassImageOrPrintOptionsDemo
{
public static void Run()
{
// Create ImageOrPrintOptions and set properties
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
// Create a new workbook with sample data and chart
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Save chart as image using the options
chart.ToImage("output_chart.png", options);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
