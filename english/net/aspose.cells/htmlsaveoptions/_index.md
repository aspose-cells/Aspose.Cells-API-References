---
title: HtmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 3730
url: /net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Represents the options for saving html file.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Creates options for saving html file. |
| [HtmlSaveOptions](htmlsaveoptions)(SaveFormat) | Creates options for saving htm file. |

## Properties

| Name | Description |
| --- | --- |
| [AddTooltipText](addtooltiptext) { get; set; } | Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false. |
| [AttachedFilesDirectory](attachedfilesdirectory) { get; set; } | The directory that the attached files will be saved to. Only for saving to html stream. |
| [AttachedFilesUrlPrefix](attachedfilesurlprefix) { get; set; } | Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream. |
| [CellCssPrefix](cellcssprefix) { get; set; } | Gets and sets the prefix of the css name,the default value is "". |
| [DefaultFontName](defaultfontname) { get; set; } | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [DisableDownlevelRevealedComments](disabledownlevelrevealedcomments) { get; set; } | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [Encoding](encoding) { get; set; } | If not set,use Encoding.UTF8 as default enconding type. |
| [ExcludeUnusedStyles](excludeunusedstyles) { get; set; } | Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false. |
| [ExportActiveWorksheetOnly](exportactiveworksheetonly) { get; set; } | Indicates if exporting the whole workbook to html file. |
| [ExportArea](exportarea) { get; set; } | Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html. |
| [ExportBogusRowData](exportbogusrowdata) { get; set; } | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportCellCoordinate](exportcellcoordinate) { get; set; } | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value. |
| [ExportDataOptions](exportdataoptions) { get; set; } | Indicating the rule of exporting html file data.The default value is All. |
| [ExportDocumentProperties](exportdocumentproperties) { get; set; } | Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportExtraHeadings](exportextraheadings) { get; set; } | Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value. |
| [ExportFormula](exportformula) { get; set; } | Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value. |
| [ExportFrameScriptsAndProperties](exportframescriptsandproperties) { get; set; } | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportGridLines](exportgridlines) { get; set; } | Indicating whether exporting the gridlines.The default value is false. |
| [ExportHeadings](exportheadings) { get; set; } | Indicates whether exporting headings when saving file to html.The default value is false. If you want to import the html file to excel, please keep the default value. |
| [ExportHiddenWorksheet](exporthiddenworksheet) { get; set; } | Indicating if exporting the hidden worksheet content.The default value is true. |
| [ExportImagesAsBase64](exportimagesasbase64) { get; set; } | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [ExportPrintAreaOnly](exportprintareaonly) { get; set; } | Indicates if only exporting the print area to html file. The default value is false. |
| [ExportSimilarBorderStyle](exportsimilarborderstyle) { get; set; } | Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false. |
| [ExportSingleTab](exportsingletab) { get; set; } | Indicates whether exporting the single tab when the file only has one worksheet. The default value is false. |
| [ExportWorkbookProperties](exportworkbookproperties) { get; set; } | Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [ExportWorksheetCSSSeparately](exportworksheetcssseparately) { get; set; } | Indicating whether export the worksheet css separately.The default value is false. |
| [ExportWorksheetProperties](exportworksheetproperties) { get; set; } | Indicating whether exporting worksheet properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value. |
| [FilePathProvider](filepathprovider) { get; set; } | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [HiddenColDisplayType](hiddencoldisplaytype) { get; set; } | Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [HiddenRowDisplayType](hiddenrowdisplaytype) { get; set; } | Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [HtmlCrossStringType](htmlcrossstringtype) { get; set; } | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [IgnoreInvisibleShapes](ignoreinvisibleshapes) { get; set; } | Indicate whether exporting those not visible shapes |
| [ImageOptions](imageoptions) { get; } | Get the ImageOrPrintOptions object before exporting |
| [ImageScalable](imagescalable) { get; set; } | Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true. |
| [IsExpImageToTempDir](isexpimagetotempdir) { get; set; } | Indicates whether exporting image files to temp directory. Only for saving to html stream. |
| [IsExportComments](isexportcomments) { get; set; } | Indicates if exporting comments when saving file to html, the default value is false. |
| [IsFullPathLink](isfullpathlink) { get; set; } | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false. |
| [LinkTargetType](linktargettype) { get; set; } | Indicating the type of target attribute in &lt;a&gt; link,The default value is HtmlLinkTargetType.Parent. |
| [MergeEmptyTdForcely](mergeemptytdforcely) { get; set; } | Indicates whether merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. The default value is false. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
| [PageTitle](pagetitle) { get; set; } | The title of the html page. Only for saving to html stream. |
| [ParseHtmlTagInCell](parsehtmltagincell) { get; set; } | Parse html tag in cell,like ,as cell value,or as html tag,default is true |
| [PresentationPreference](presentationpreference) { get; set; } | Indicating if html or mht file is presentation preference.The default value is false.if you want to get more beautiful presentation,please set the value to true. |
| [SaveAsSingleFile](saveassinglefile) { get; set; } | Indicates whether save the html as single file. The default value is false. |
| [StreamProvider](streamprovider) { get; set; } | Gets or sets the IStreamProvider for exporting objects. |
| [TableCssId](tablecssid) { get; set; } | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "". |
| [WidthScalable](widthscalable) { get; set; } | Indicates whether using scalable unit to describe the column width when exporting file to html. The default value is false. |
| [WorksheetScalable](worksheetscalable) { get; set; } | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |

### See Also

* class [SaveOptions](../saveoptions)
* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
