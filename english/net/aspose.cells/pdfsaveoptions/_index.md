---
title: PdfSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 4490
url: /net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Represents the options for saving pdf file.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Creates the options for saving pdf file. |

## Properties

| Name | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](allcolumnsinonepagepersheet) { get; set; } | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [Bookmark](bookmark) { get; set; } | Gets and sets the [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry) object. |
| [CalculateFormula](calculateformula) { get; set; } | Indicates whether to calculate formulas before saving pdf file. |
| [CheckFontCompatibility](checkfontcompatibility) { get; set; } | Indicates whether to check font compatibility for every character in text. |
| [CheckWorkbookDefaultFont](checkworkbookdefaultfont) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [Compliance](compliance) { get; set; } | Workbook converts to pdf will according to PdfCompliance in this property. |
| [CreatedTime](createdtime) { get; set; } | Gets and sets the time of generating the pdf document. |
| [CustomPropertiesExport](custompropertiesexport) { get; set; } | Gets or sets a value determining the way [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) are exported to PDF file. Default value is None. |
| [DefaultEditLanguage](defaulteditlanguage) { get; set; } | Gets or sets default edit language. |
| [DefaultFont](defaultfont) { get; set; } | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [DisplayDocTitle](displaydoctitle) { get; set; } | Indicates whether the window's title bar should display the document title. |
| [DrawObjectEventHandler](drawobjecteventhandler) { get; set; } | Implements this interface to get DrawObject and Bound when rendering. |
| [EmbedStandardWindowsFonts](embedstandardwindowsfonts) { get; set; } | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [EmfRenderSetting](emfrendersetting) { get; set; } | Setting for rendering Emf metafile. |
| [ExportDocumentStructure](exportdocumentstructure) { get; set; } | Indicates whether to export document structure. |
| [FontEncoding](fontencoding) { get; set; } | Gets or sets embedded font encoding in pdf. |
| [GridlineType](gridlinetype) { get; set; } | Gets or sets gridline type. |
| [IgnoreError](ignoreerror) { get; set; } | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [ImageType](imagetype) { get; set; } | Represents the image type when converting the chart and shape . |
| [IsFontSubstitutionCharGranularity](isfontsubstitutionchargranularity) { get; set; } | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [OnePagePerSheet](onepagepersheet) { get; set; } | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [OptimizationType](optimizationtype) { get; set; } | Gets and sets pdf optimization type. |
| [OutputBlankPageWhenNothingToPrint](outputblankpagewhennothingtoprint) { get; set; } | Indicates whether to output a blank page when there is nothing to print. |
| [PageCount](pagecount) { get; set; } | Gets or sets the number of pages to save. |
| [PageIndex](pageindex) { get; set; } | Gets or sets the 0-based index of the first page to save. |
| [PageSavingCallback](pagesavingcallback) { get; set; } | Control/Indicate progress of page saving process. |
| [PdfCompression](pdfcompression) { get; set; } | Indicate the compression algorithm |
| [PrintingPageType](printingpagetype) { get; set; } | Indicates which pages will not be printed. |
| [Producer](producer) { get; set; } | Gets and sets producer of generated pdf document. |
| [SecurityOptions](securityoptions) { get; set; } | Set this options, when security is need in xls2pdf result. |
| [TextCrossType](textcrosstype) { get; set; } | Gets or sets displaying text type when the text width is larger than cell width. |

## Methods

| Name | Description |
| --- | --- |
| [SetImageResample](setimageresample)(int, int) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled. |

### See Also

* class [SaveOptions](../saveoptions)
* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
