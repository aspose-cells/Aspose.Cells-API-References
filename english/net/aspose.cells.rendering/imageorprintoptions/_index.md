---
title: ImageOrPrintOptions
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 5130
url: /net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.

```csharp
public class ImageOrPrintOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](allcolumnsinonepagepersheet) { get; set; } | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [ChartImageType](chartimagetype) { get; set; } | Indicate the chart imagetype when converting. default value: PNG. |
| [CheckWorkbookDefaultFont](checkworkbookdefaultfont) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [CustomPrintPageEventHandler](customprintpageeventhandler) { get; set; } | Client can special output to printer when print each page using this EventHandler |
| [CustomQueryPageSettingsEventHandler](customquerypagesettingseventhandler) { get; set; } | Client can control page setting of printer when print each page using this EventHandler |
| [DefaultEditLanguage](defaulteditlanguage) { get; set; } | Gets or sets default edit language. |
| [DefaultFont](defaultfont) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [DrawObjectEventHandler](drawobjecteventhandler) { get; set; } | Implements this interface to get DrawObject and Bound when rendering. |
| [EmbededImageNameInSvg](embededimagenameinsvg) { get; set; } | Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [EmfType](emftype) { get; set; } | Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual. |
| [GridlineType](gridlinetype) { get; set; } | Gets or sets gridline type. |
| [HorizontalResolution](horizontalresolution) { get; set; } | Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. |
| [ImageType](imagetype) { get; set; } | Gets or sets the format of the generated images. default value: PNG. |
| [IsCellAutoFit](iscellautofit) { get; set; } | Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. |
| [IsFontSubstitutionCharGranularity](isfontsubstitutionchargranularity) { get; set; } | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [IsOptimized](isoptimized) { get; set; } | Indicates whether to optimize the output elements. |
| [OnePagePerSheet](onepagepersheet) { get; set; } | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [OnlyArea](onlyarea) { get; set; } | If this property is true , one Area will be output, and no scale will take effect. |
| [OutputBlankPageWhenNothingToPrint](outputblankpagewhennothingtoprint) { get; set; } | Indicates whether to output a blank page when there is nothing to print. |
| [PageCount](pagecount) { get; set; } | Gets or sets the number of pages to save. |
| [PageIndex](pageindex) { get; set; } | Gets or sets the 0-based index of the first page to save. |
| [PageSavingCallback](pagesavingcallback) { get; set; } | Control/Indicate progress of page saving process. |
| [PixelFormat](pixelformat) { get; set; } | Gets or sets the pixel format for the generated images. |
| [PrintingPage](printingpage) { get; set; } | Indicates which pages will not be printed. |
| [PrintWithStatusDialog](printwithstatusdialog) { get; set; } | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [Quality](quality) { get; set; } | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. The default value is 100 |
| [SaveFormat](saveformat) { get; set; } | Gets or sets the output file format type Support Tiff/XPS |
| [SmoothingMode](smoothingmode) { get; set; } | Specifies whether smoothing (antialiasing) is applied to lines and curves and the edges of filled areas. The default value is SmoothingMode.None |
| [SVGFitToViewPort](svgfittoviewport) { get; set; } | if this property is true, the generated svg will fit to view port. |
| [TextCrossType](textcrosstype) { get; set; } | Gets or sets displaying text type when the text width is larger than cell width. |
| [TextRenderingHint](textrenderinghint) { get; set; } | Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault |
| [TiffColorDepth](tiffcolordepth) { get; set; } | Gets or sets bit depth to apply only when saving pages to the `Tiff` format. |
| [TiffCompression](tiffcompression) { get; set; } | Gets or sets the type of compression to apply only when saving pages to the `Tiff` format. |
| [Transparent](transparent) { get; set; } | Indicates if the background of generated image should be transparent. |
| [VerticalResolution](verticalresolution) { get; set; } | Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf format image. |
| [WarningCallback](warningcallback) { get; set; } | Gets or sets warning callback. |

## Methods

| Name | Description |
| --- | --- |
| [SetDesiredSize](setdesiredsize)(int, int) | Sets desired width and height of image. |

### Examples

```csharp

[C#]

//Set Image Or Print Options
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Set output image format
options.ImageType = ImageType.Png;

//Set Horizontal resolution
options.HorizontalResolution = 300;

//Set Vertical Resolution
options.VerticalResolution = 300;

//Instantiate Workbook
Workbook book = new Workbook("test.xls");

//Save chart as Image using ImageOrPrint Options
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Set Image Or Print Options
Dim options As New ImageOrPrintOptions()

'Set output image format
options.ImageType = ImageType.Png

'Set Horizontal resolution
options.HorizontalResolution = 300

'Set Vertical Resolution
options.VerticalResolution = 300

'Instantiate Workbook
Dim book As New Workbook("test.xls")

'Save chart as Image using ImageOrPrint Options
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
