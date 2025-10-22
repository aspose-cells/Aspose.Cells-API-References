##PageSetup Class
'PageSetup class. Encapsulates the object that represents pagesetup in Go.'
## PageSetup class
Encapsulates the object that represents the page setup description.The PageSetup object contains all page setup options.
```go
type PageSetup struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetODSPageBackground](./getodspagebackground/) | Gets the background of ODS. |
|[Copy](./copy/) | Copies the setting of the page setup. |
|[GetPrintArea](./getprintarea/) | Represents the range to be printed. |
|[SetPrintArea](./setprintarea/) | Represents the range to be printed. |
|[GetPrintTitleColumns](./getprinttitlecolumns/) | Represents the columns that contain the cells to be repeated on the left side of each page. |
|[SetPrintTitleColumns](./setprinttitlecolumns/) | Represents the columns that contain the cells to be repeated on the left side of each page. |
|[GetPrintTitleRows](./getprinttitlerows/) | Represents the rows that contain the cells to be repeated at the top of each page. |
|[SetPrintTitleRows](./setprinttitlerows/) | Represents the rows that contain the cells to be repeated at the top of each page. |
|[GetBlackAndWhite](./getblackandwhite/) | Represents if elements of the document will be printed in black and white. |
|[SetBlackAndWhite](./setblackandwhite/) | Represents if elements of the document will be printed in black and white. |
|[GetCenterHorizontally](./getcenterhorizontally/) | Represent if the sheet is printed centered horizontally. |
|[SetCenterHorizontally](./setcenterhorizontally/) | Represent if the sheet is printed centered horizontally. |
|[GetCenterVertically](./getcentervertically/) | Represent if the sheet is printed centered vertically. |
|[SetCenterVertically](./setcentervertically/) | Represent if the sheet is printed centered vertically. |
|[GetPrintDraft](./getprintdraft/) | Represents if the sheet will be printed without graphics. |
|[SetPrintDraft](./setprintdraft/) | Represents if the sheet will be printed without graphics. |
|[GetFooterMargin](./getfootermargin/) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
|[SetFooterMargin](./setfootermargin/) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
|[GetFooterMarginInch](./getfootermargininch/) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
|[SetFooterMarginInch](./setfootermargininch/) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
|[GetHeaderMargin](./getheadermargin/) | Represents the distance from the top of the page to the header, in unit of centimeters. |
|[SetHeaderMargin](./setheadermargin/) | Represents the distance from the top of the page to the header, in unit of centimeters. |
|[GetHeaderMarginInch](./getheadermargininch/) | Represents the distance from the top of the page to the header, in unit of inches. |
|[SetHeaderMarginInch](./setheadermargininch/) | Represents the distance from the top of the page to the header, in unit of inches. |
|[GetPrinterSettings](./getprintersettings/) | Gets and sets the settings of the default printer. |
|[SetPrinterSettings](./setprintersettings/) | Gets and sets the settings of the default printer. |
|[GetLeftMargin](./getleftmargin/) | Represents the size of the left margin, in unit of centimeters. |
|[SetLeftMargin](./setleftmargin/) | Represents the size of the left margin, in unit of centimeters. |
|[GetLeftMarginInch](./getleftmargininch/) | Represents the size of the left margin, in unit of inches. |
|[SetLeftMarginInch](./setleftmargininch/) | Represents the size of the left margin, in unit of inches. |
|[GetRightMargin](./getrightmargin/) | Represents the size of the right margin, in unit of centimeters. |
|[SetRightMargin](./setrightmargin/) | Represents the size of the right margin, in unit of centimeters. |
|[GetRightMarginInch](./getrightmargininch/) | Represents the size of the right margin, in unit of inches. |
|[SetRightMarginInch](./setrightmargininch/) | Represents the size of the right margin, in unit of inches. |
|[GetTopMargin](./gettopmargin/) | Represents the size of the top margin, in unit of centimeters. |
|[SetTopMargin](./settopmargin/) | Represents the size of the top margin, in unit of centimeters. |
|[GetTopMarginInch](./gettopmargininch/) | Represents the size of the top margin, in unit of inches. |
|[SetTopMarginInch](./settopmargininch/) | Represents the size of the top margin, in unit of inches. |
|[GetBottomMargin](./getbottommargin/) | Represents the size of the bottom margin, in unit of centimeters. |
|[SetBottomMargin](./setbottommargin/) | Represents the size of the bottom margin, in unit of centimeters. |
|[GetBottomMarginInch](./getbottommargininch/) | Represents the size of the bottom margin, in unit of inches. |
|[SetBottomMarginInch](./setbottommargininch/) | Represents the size of the bottom margin, in unit of inches. |
|[GetFirstPageNumber](./getfirstpagenumber/) | Represents the first page number that will be used when this sheet is printed. |
|[SetFirstPageNumber](./setfirstpagenumber/) | Represents the first page number that will be used when this sheet is printed. |
|[SetFitToPages](./setfittopages/) | Sets the number of pages the worksheet will be scaled to when it's printed. |
|[GetFitToPagesTall](./getfittopagestall/) | Represents  the number of pages tall the worksheet will be scaled to when it's printed.The default value is 1. |
|[SetFitToPagesTall](./setfittopagestall/) | Represents  the number of pages tall the worksheet will be scaled to when it's printed.The default value is 1. |
|[GetFitToPagesWide](./getfittopageswide/) | Represents the number of pages wide the worksheet will be scaled to when it's printed.The default value is 1. |
|[SetFitToPagesWide](./setfittopageswide/) | Represents the number of pages wide the worksheet will be scaled to when it's printed.The default value is 1. |
|[IsPercentScale](./ispercentscale/) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
|[SetIsPercentScale](./setispercentscale/) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
|[GetOrder](./getorder/) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
|[SetOrder](./setorder/) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
|[IsAutomaticPaperSize](./isautomaticpapersize/) | Indicates whether the paper size is automatic. |
|[GetPaperSize](./getpapersize/) | Represents the size of the paper. |
|[SetPaperSize](./setpapersize/) | Represents the size of the paper. |
|[GetPaperWidth](./getpaperwidth/) | Gets the width of the paper in unit of inches, considered page orientation. |
|[GetPaperHeight](./getpaperheight/) | Gets the height of the paper in unit of inches , considered page orientation. |
|[CustomPaperSize](./custompapersize/) | Sets the custom paper size, in unit of inches. |
|[GetOrientation](./getorientation/) | Represents page print orientation. |
|[SetOrientation](./setorientation/) | Represents page print orientation. |
|[GetPrintComments](./getprintcomments/) | Represents the way comments are printed with the sheet. |
|[SetPrintComments](./setprintcomments/) | Represents the way comments are printed with the sheet. |
|[GetPrintErrors](./getprinterrors/) | Specifies the type of print error displayed. |
|[SetPrintErrors](./setprinterrors/) | Specifies the type of print error displayed. |
|[GetPrintHeadings](./getprintheadings/) | Represents if row and column headings are printed with this page. |
|[SetPrintHeadings](./setprintheadings/) | Represents if row and column headings are printed with this page. |
|[GetPrintGridlines](./getprintgridlines/) | Represents if cell gridlines are printed on the page. |
|[SetPrintGridlines](./setprintgridlines/) | Represents if cell gridlines are printed on the page. |
|[GetZoom](./getzoom/) | Represents the scaling factor in percent. It should be between 10 and 400. |
|[SetZoom](./setzoom/) | Represents the scaling factor in percent. It should be between 10 and 400. |
|[IsAutoFirstPageNumber](./isautofirstpagenumber/) | Indicates whether the first the page number is automatically assigned. |
|[SetIsAutoFirstPageNumber](./setisautofirstpagenumber/) | Indicates whether the first the page number is automatically assigned. |
|[GetPrintQuality](./getprintquality/) | Represents the print quality. |
|[SetPrintQuality](./setprintquality/) | Represents the print quality. |
|[GetPrintCopies](./getprintcopies/) | Get and sets number of copies to print. |
|[SetPrintCopies](./setprintcopies/) | Get and sets number of copies to print. |
|[ClearHeaderFooter](./clearheaderfooter/) | Clears header and footer setting. |
|[GetHeader](./getheader/) | Gets a script formatting the header of an Excel file. |
|[GetCommands](./getcommands/) | Gets all commands of header or footer. |
|[GetFooter](./getfooter/) | Gets a script formatting the footer of an Excel file. |
|[SetHeader](./setheader/) | Sets a script formatting the header of an Excel file. |
|[SetFooter](./setfooter/) | Sets a script formatting the footer of an Excel file. |
|[SetEvenHeader](./setevenheader/) | Sets a script formatting the even page header of an Excel file.Only effect in Excel 2007 when IsHFDiffOddEven is true. |
|[GetEvenHeader](./getevenheader/) | Gets a script formatting the even header of an Excel file. |
|[SetEvenFooter](./setevenfooter/) | Sets a script formatting the even page footer of an Excel file.Only effect in Excel 2007 when IsHFDiffOddEven is true. |
|[GetEvenFooter](./getevenfooter/) | Gets a script formatting the even footer of an Excel file. |
|[SetFirstPageHeader](./setfirstpageheader/) | Sets a script formatting the first page header of an Excel file.Only effect in Excel 2007 when IsHFDiffFirst is true. |
|[GetFirstPageHeader](./getfirstpageheader/) | Gets a script formatting the first page header of an Excel file. |
|[SetFirstPageFooter](./setfirstpagefooter/) | Sets a script formatting the first page footer of an Excel file. |
|[GetFirstPageFooter](./getfirstpagefooter/) | Gets a script formatting the first page footer of an Excel file. |
|[IsHFDiffOddEven](./ishfdiffoddeven/) | True means that the header/footer of the odd pages is different with odd pages. |
|[SetIsHFDiffOddEven](./setishfdiffoddeven/) | True means that the header/footer of the odd pages is different with odd pages. |
|[IsHFDiffFirst](./ishfdifffirst/) | True means that the header/footer of the first page is different with other pages. |
|[SetIsHFDiffFirst](./setishfdifffirst/) | True means that the header/footer of the first page is different with other pages. |
|[IsHFScaleWithDoc](./ishfscalewithdoc/) | Indicates whether header and footer are scaled with document scaling.Only applies for Excel 2007. |
|[SetIsHFScaleWithDoc](./setishfscalewithdoc/) | Indicates whether header and footer are scaled with document scaling.Only applies for Excel 2007. |
|[IsHFAlignMargins](./ishfalignmargins/) | Indicates whether header and footer margins are aligned with the page margins.If this property is true, the left header and footer will be aligned with the left margin,and the right header and footer will be aligned with the right margin.This option is enabled by default. |
|[SetIsHFAlignMargins](./setishfalignmargins/) | Indicates whether header and footer margins are aligned with the page margins.If this property is true, the left header and footer will be aligned with the left margin,and the right header and footer will be aligned with the right margin.This option is enabled by default. |
|[SetHeaderPicture](./setheaderpicture/) | Sets an image in the header of a worksheet. |
|[SetFooterPicture](./setfooterpicture/) | Sets an image in the footer of a worksheet. |
|[SetPicture](./setpicture/) | Sets an image in the header/footer of a worksheet. |
|[GetPicture_Bool_Int](./getpicture_bool_int/) | Gets the Picture object of the header / footer. |
|[GetPicture_Bool_Bool_Bool_Int](./getpicture_bool_bool_bool_int/) | Gets the Picture object of the header / footer. |
