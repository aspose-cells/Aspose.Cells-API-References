---
title: PageSetup
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 4390
url: /net/aspose.cells/pagesetup/
---
## PageSetup class

Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.

```csharp
public class PageSetup
```

## Properties

| Name | Description |
| --- | --- |
| [BlackAndWhite](blackandwhite) { get; set; } | Represents if elements of the document will be printed in black and white. |
| [BottomMargin](bottommargin) { get; set; } | Represents the size of the bottom margin, in unit of centimeters. |
| [BottomMarginInch](bottommargininch) { get; set; } | Represents the size of the bottom margin, in unit of inches. |
| [CenterHorizontally](centerhorizontally) { get; set; } | Represent if the sheet is printed centered horizontally. |
| [CenterVertically](centervertically) { get; set; } | Represent if the sheet is printed centered vertically. |
| [FirstPageNumber](firstpagenumber) { get; set; } | Represents the first page number that will be used when this sheet is printed. |
| [FitToPagesTall](fittopagestall) { get; set; } | Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [FitToPagesWide](fittopageswide) { get; set; } | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [FooterMargin](footermargin) { get; set; } | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [FooterMarginInch](footermargininch) { get; set; } | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [HeaderMargin](headermargin) { get; set; } | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [HeaderMarginInch](headermargininch) { get; set; } | Represents the distance from the top of the page to the header, in unit of inches. |
| [IsAutoFirstPageNumber](isautofirstpagenumber) { get; set; } | Indicates whether the first the page number is automatically assigned. |
| [IsAutomaticPaperSize](isautomaticpapersize) { get; } | Indicates whether the paper size is automatic. |
| [IsHFAlignMargins](ishfalignmargins) { get; set; } | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
| [IsHFDiffFirst](ishfdifffirst) { get; set; } | True means that the header/footer of the first page is different with other pages. |
| [IsHFDiffOddEven](ishfdiffoddeven) { get; set; } | True means that the header/footer of the odd pages is different with odd pages. |
| [IsHFScaleWithDoc](ishfscalewithdoc) { get; set; } | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [IsPercentScale](ispercentscale) { get; set; } | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [LeftMargin](leftmargin) { get; set; } | Represents the size of the left margin, in unit of centimeters. |
| [LeftMarginInch](leftmargininch) { get; set; } | Represents the size of the left margin, in unit of inches. |
| [ODSPageBackground](odspagebackground) { get; } | Gets the background of ODS. |
| [Order](order) { get; set; } | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [Orientation](orientation) { get; set; } | Represents page print orientation. |
| [PaperHeight](paperheight) { get; } | Gets the height of the paper in unit of inches , considered page orientation. |
| [PaperSize](papersize) { get; set; } | Represents the size of the paper. |
| [PaperWidth](paperwidth) { get; } | Gets the width of the paper in unit of inches, considered page orientation. |
| [PrintArea](printarea) { get; set; } | Represents the range to be printed. |
| [PrintComments](printcomments) { get; set; } | Represents the way comments are printed with the sheet. |
| [PrintCopies](printcopies) { get; set; } | Get and sets number of copies to print. |
| [PrintDraft](printdraft) { get; set; } | Represents if the sheet will be printed without graphics. |
| [PrintErrors](printerrors) { get; set; } | Specifies the type of print error displayed. |
| [PrinterSettings](printersettings) { get; set; } | Gets and sets the settings of the default printer. |
| [PrintGridlines](printgridlines) { get; set; } | Represents if cell gridlines are printed on the page. |
| [PrintHeadings](printheadings) { get; set; } | Represents if row and column headings are printed with this page. |
| [PrintQuality](printquality) { get; set; } | Represents the print quality. |
| [PrintTitleColumns](printtitlecolumns) { get; set; } | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [PrintTitleRows](printtitlerows) { get; set; } | Represents the rows that contain the cells to be repeated at the top of each page. |
| [RightMargin](rightmargin) { get; set; } | Represents the size of the right margin, in unit of centimeters. |
| [RightMarginInch](rightmargininch) { get; set; } | Represents the size of the right margin, in unit of inches. |
| [TopMargin](topmargin) { get; set; } | Represents the size of the top margin, in unit of centimeters. |
| [TopMarginInch](topmargininch) { get; set; } | Represents the size of the top margin, in unit of inches. |
| [Zoom](zoom) { get; set; } | Represents the scaling factor in percent. It should be between 10 and 400. |

## Methods

| Name | Description |
| --- | --- |
| [ClearHeaderFooter](clearheaderfooter)() | Clears header and footer setting. |
| [Copy](copy)(PageSetup, CopyOptions) | Copies the setting of the page setup. |
| [CustomPaperSize](custompapersize)(double, double) | Sets the custom paper size, in unit of inches. |
| [GetCommands](getcommands)(string) | Gets all commands of header or footer. |
| [GetEvenFooter](getevenfooter)(int) | Gets a script formatting the even footer of an Excel file. |
| [GetEvenHeader](getevenheader)(int) | Gets a script formatting the even header of an Excel file. |
| [GetFirstPageFooter](getfirstpagefooter)(int) | Gets a script formatting the first page footer of an Excel file. |
| [GetFirstPageHeader](getfirstpageheader)(int) | Gets a script formatting the first page header of an Excel file. |
| [GetFooter](getfooter)(int) | Gets a script formatting the footer of an Excel file. |
| [GetHeader](getheader)(int) | Gets a script formatting the header of an Excel file. |
| [GetPicture](getpicture)(bool, int) | Gets the [`Picture`](../../aspose.cells.drawing/picture) object of the header / footer. |
| [GetPicture](getpicture)(bool, bool, bool, int) | Gets the [`Picture`](../../aspose.cells.drawing/picture) object of the header / footer. |
| [SetEvenFooter](setevenfooter)(int, string) | Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [SetEvenHeader](setevenheader)(int, string) | Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [SetFirstPageFooter](setfirstpagefooter)(int, string) | Sets a script formatting the first page footer of an Excel file. |
| [SetFirstPageHeader](setfirstpageheader)(int, string) | Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true. |
| [SetFitToPages](setfittopages)(int, int) | Sets the number of pages the worksheet will be scaled to when it's printed. |
| [SetFooter](setfooter)(int, string) | Sets a script formatting the footer of an Excel file. |
| [SetFooterPicture](setfooterpicture)(int, byte[]) | Sets an image in the footer of a worksheet. |
| [SetHeader](setheader)(int, string) | Sets a script formatting the header of an Excel file. |
| [SetHeaderPicture](setheaderpicture)(int, byte[]) | Sets an image in the header of a worksheet. |
| [SetPicture](setpicture)(bool, bool, bool, int, byte[]) | Sets an image in the header/footer of a worksheet. |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Add a worksheet
sheets.Add();
Worksheet sheet = sheets[1];
PageSetup pageSetup = sheet.PageSetup;
pageSetup.PrintArea = "D1:K13";

//do your business

[Visual Basic]
Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Add a worksheet
sheets.Add()
Dim sheet as Worksheet = sheets(1)
Dim pageSetup as PageSetup = sheet.PageSetup
pageSetup.PrintArea = "D1:K13"
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
