##Aspose::Cells::PageSetup class
'Aspose::Cells::PageSetup class. Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options in C++.'
## PageSetup class
Encapsulates the object that represents the page setup description. The [PageSetup](./) object contains all page setup options.
```cpp
class PageSetup
```
## Methods
| Method | Description |
| --- | --- |
| [ClearHeaderFooter()](./clearheaderfooter/) | Clears header and footer setting. |
| [Copy(const PageSetup\& source, const CopyOptions\& copyOptions)](./copy/) | Copies the setting of the page setup. |
| [CustomPaperSize(double width, double height)](./custompapersize/) | Sets the custom paper size, in unit of inches. |
| [GetBlackAndWhite()](./getblackandwhite/) | Represents if elements of the document will be printed in black and white. |
| [GetBottomMargin()](./getbottommargin/) | Represents the size of the bottom margin, in unit of centimeters. |
| [GetBottomMarginInch()](./getbottommargininch/) | Represents the size of the bottom margin, in unit of inches. |
| [GetCenterHorizontally()](./getcenterhorizontally/) | Represent if the sheet is printed centered horizontally. |
| [GetCenterVertically()](./getcentervertically/) | Represent if the sheet is printed centered vertically. |
| [GetCommands(const U16String\& headerFooterScript)](./getcommands/) | Gets all commands of header or footer. |
| [GetCommands(const char16_t* headerFooterScript)](./getcommands/) | Gets all commands of header or footer. |
| [GetEvenFooter(int32_t section)](./getevenfooter/) | Gets a script formatting the even footer of an Excel file. |
| [GetEvenHeader(int32_t section)](./getevenheader/) | Gets a script formatting the even header of an Excel file. |
| [GetFirstPageFooter(int32_t section)](./getfirstpagefooter/) | Gets a script formatting the first page footer of an Excel file. |
| [GetFirstPageHeader(int32_t section)](./getfirstpageheader/) | Gets a script formatting the first page header of an Excel file. |
| [GetFirstPageNumber()](./getfirstpagenumber/) | Represents the first page number that will be used when this sheet is printed. |
| [GetFitToPagesTall()](./getfittopagestall/) | Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [GetFitToPagesWide()](./getfittopageswide/) | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [GetFooter(int32_t section)](./getfooter/) | Gets a script formatting the footer of an Excel file. |
| [GetFooterMargin()](./getfootermargin/) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [GetFooterMarginInch()](./getfootermargininch/) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [GetHeader(int32_t section)](./getheader/) | Gets a script formatting the header of an Excel file. |
| [GetHeaderMargin()](./getheadermargin/) | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [GetHeaderMarginInch()](./getheadermargininch/) | Represents the distance from the top of the page to the header, in unit of inches. |
| [GetLeftMargin()](./getleftmargin/) | Represents the size of the left margin, in unit of centimeters. |
| [GetLeftMarginInch()](./getleftmargininch/) | Represents the size of the left margin, in unit of inches. |
| [GetODSPageBackground()](./getodspagebackground/) | Gets the background of ODS. |
| [GetOrder()](./getorder/) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [GetOrientation()](./getorientation/) | Represents page print orientation. |
| [GetPaperHeight()](./getpaperheight/) | Gets the height of the paper in unit of inches , considered page orientation. |
| [GetPaperSize()](./getpapersize/) | Represents the size of the paper. |
| [GetPaperWidth()](./getpaperwidth/) | Gets the width of the paper in unit of inches, considered page orientation. |
| [GetPicture(bool isHeader, int32_t section)](./getpicture/) | Gets the Picture object of the header / footer. |
| [GetPicture(bool isFirst, bool isEven, bool isHeader, int32_t section)](./getpicture/) | Gets the Picture object of the header / footer. |
| [GetPrintArea()](./getprintarea/) | Represents the range to be printed. |
| [GetPrintComments()](./getprintcomments/) | Represents the way comments are printed with the sheet. |
| [GetPrintCopies()](./getprintcopies/) | Get and sets number of copies to print. |
| [GetPrintDraft()](./getprintdraft/) | Represents if the sheet will be printed without graphics. |
| [GetPrintErrors()](./getprinterrors/) | Specifies the type of print error displayed. |
| [GetPrinterSettings()](./getprintersettings/) | Gets and sets the settings of the default printer. |
| [GetPrintGridlines()](./getprintgridlines/) | Represents if cell gridlines are printed on the page. |
| [GetPrintHeadings()](./getprintheadings/) | Represents if row and column headings are printed with this page. |
| [GetPrintQuality()](./getprintquality/) | Represents the print quality. |
| [GetPrintTitleColumns()](./getprinttitlecolumns/) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [GetPrintTitleRows()](./getprinttitlerows/) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [GetRightMargin()](./getrightmargin/) | Represents the size of the right margin, in unit of centimeters. |
| [GetRightMarginInch()](./getrightmargininch/) | Represents the size of the right margin, in unit of inches. |
| [GetTopMargin()](./gettopmargin/) | Represents the size of the top margin, in unit of centimeters. |
| [GetTopMarginInch()](./gettopmargininch/) | Represents the size of the top margin, in unit of inches. |
| [GetZoom()](./getzoom/) | Represents the scaling factor in percent. It should be between 10 and 400. |
| [IsAutoFirstPageNumber()](./isautofirstpagenumber/) | Indicates whether the first the page number is automatically assigned. |
| [IsAutomaticPaperSize()](./isautomaticpapersize/) | Indicates whether the paper size is automatic. |
| [IsHFAlignMargins()](./ishfalignmargins/) | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
| [IsHFDiffFirst()](./ishfdifffirst/) | True means that the header/footer of the first page is different with other pages. |
| [IsHFDiffOddEven()](./ishfdiffoddeven/) | True means that the header/footer of the odd pages is different with odd pages. |
| [IsHFScaleWithDoc()](./ishfscalewithdoc/) | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsPercentScale()](./ispercentscale/) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PageSetup\& src)](./operator_asm/) | operator= |
| [PageSetup(PageSetup_Impl* impl)](./pagesetup/) | Constructs from an implementation object. |
| [PageSetup(const PageSetup\& src)](./pagesetup/) | Copy constructor. |
| [SetBlackAndWhite(bool value)](./setblackandwhite/) | Represents if elements of the document will be printed in black and white. |
| [SetBottomMargin(double value)](./setbottommargin/) | Represents the size of the bottom margin, in unit of centimeters. |
| [SetBottomMarginInch(double value)](./setbottommargininch/) | Represents the size of the bottom margin, in unit of inches. |
| [SetCenterHorizontally(bool value)](./setcenterhorizontally/) | Represent if the sheet is printed centered horizontally. |
| [SetCenterVertically(bool value)](./setcentervertically/) | Represent if the sheet is printed centered vertically. |
| [SetEvenFooter(int32_t section, const U16String\& footerScript)](./setevenfooter/) | Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [SetEvenFooter(int32_t section, const char16_t* footerScript)](./setevenfooter/) | Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [SetEvenHeader(int32_t section, const U16String\& headerScript)](./setevenheader/) | Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [SetEvenHeader(int32_t section, const char16_t* headerScript)](./setevenheader/) | Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [SetFirstPageFooter(int32_t section, const U16String\& footerScript)](./setfirstpagefooter/) | Sets a script formatting the first page footer of an Excel file. |
| [SetFirstPageFooter(int32_t section, const char16_t* footerScript)](./setfirstpagefooter/) | Sets a script formatting the first page footer of an Excel file. |
| [SetFirstPageHeader(int32_t section, const U16String\& headerScript)](./setfirstpageheader/) | Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true. |
| [SetFirstPageHeader(int32_t section, const char16_t* headerScript)](./setfirstpageheader/) | Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true. |
| [SetFirstPageNumber(int32_t value)](./setfirstpagenumber/) | Represents the first page number that will be used when this sheet is printed. |
| [SetFitToPages(int32_t wide, int32_t tall)](./setfittopages/) | Sets the number of pages the worksheet will be scaled to when it's printed. |
| [SetFitToPagesTall(int32_t value)](./setfittopagestall/) | Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [SetFitToPagesWide(int32_t value)](./setfittopageswide/) | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [SetFooter(int32_t section, const U16String\& footerScript)](./setfooter/) | Sets a script formatting the footer of an Excel file. |
| [SetFooter(int32_t section, const char16_t* footerScript)](./setfooter/) | Sets a script formatting the footer of an Excel file. |
| [SetFooterMargin(double value)](./setfootermargin/) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [SetFooterMarginInch(double value)](./setfootermargininch/) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [SetFooterPicture(int32_t section, const Vector \<uint8_t\>\& footerPicture)](./setfooterpicture/) | Sets an image in the footer of a worksheet. |
| [SetHeader(int32_t section, const U16String\& headerScript)](./setheader/) | Sets a script formatting the header of an Excel file. |
| [SetHeader(int32_t section, const char16_t* headerScript)](./setheader/) | Sets a script formatting the header of an Excel file. |
| [SetHeaderMargin(double value)](./setheadermargin/) | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [SetHeaderMarginInch(double value)](./setheadermargininch/) | Represents the distance from the top of the page to the header, in unit of inches. |
| [SetHeaderPicture(int32_t section, const Vector \<uint8_t\>\& headerPicture)](./setheaderpicture/) | Sets an image in the header of a worksheet. |
| [SetIsAutoFirstPageNumber(bool value)](./setisautofirstpagenumber/) | Indicates whether the first the page number is automatically assigned. |
| [SetIsHFAlignMargins(bool value)](./setishfalignmargins/) | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
| [SetIsHFDiffFirst(bool value)](./setishfdifffirst/) | True means that the header/footer of the first page is different with other pages. |
| [SetIsHFDiffOddEven(bool value)](./setishfdiffoddeven/) | True means that the header/footer of the odd pages is different with odd pages. |
| [SetIsHFScaleWithDoc(bool value)](./setishfscalewithdoc/) | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [SetIsPercentScale(bool value)](./setispercentscale/) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [SetLeftMargin(double value)](./setleftmargin/) | Represents the size of the left margin, in unit of centimeters. |
| [SetLeftMarginInch(double value)](./setleftmargininch/) | Represents the size of the left margin, in unit of inches. |
| [SetOrder(PrintOrderType value)](./setorder/) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [SetOrientation(PageOrientationType value)](./setorientation/) | Represents page print orientation. |
| [SetPaperSize(PaperSizeType value)](./setpapersize/) | Represents the size of the paper. |
| [SetPicture(bool isFirst, bool isEven, bool isHeader, int32_t section, const Vector \<uint8_t\>\& imageData)](./setpicture/) | Sets an image in the header/footer of a worksheet. |
| [SetPrintArea(const U16String\& value)](./setprintarea/) | Represents the range to be printed. |
| [SetPrintArea(const char16_t* value)](./setprintarea/) | Represents the range to be printed. |
| [SetPrintComments(PrintCommentsType value)](./setprintcomments/) | Represents the way comments are printed with the sheet. |
| [SetPrintCopies(int32_t value)](./setprintcopies/) | Get and sets number of copies to print. |
| [SetPrintDraft(bool value)](./setprintdraft/) | Represents if the sheet will be printed without graphics. |
| [SetPrintErrors(PrintErrorsType value)](./setprinterrors/) | Specifies the type of print error displayed. |
| [SetPrinterSettings(const Vector \<uint8_t\>\& value)](./setprintersettings/) | Gets and sets the settings of the default printer. |
| [SetPrintGridlines(bool value)](./setprintgridlines/) | Represents if cell gridlines are printed on the page. |
| [SetPrintHeadings(bool value)](./setprintheadings/) | Represents if row and column headings are printed with this page. |
| [SetPrintQuality(int32_t value)](./setprintquality/) | Represents the print quality. |
| [SetPrintTitleColumns(const U16String\& value)](./setprinttitlecolumns/) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [SetPrintTitleColumns(const char16_t* value)](./setprinttitlecolumns/) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [SetPrintTitleRows(const U16String\& value)](./setprinttitlerows/) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [SetPrintTitleRows(const char16_t* value)](./setprinttitlerows/) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [SetRightMargin(double value)](./setrightmargin/) | Represents the size of the right margin, in unit of centimeters. |
| [SetRightMarginInch(double value)](./setrightmargininch/) | Represents the size of the right margin, in unit of inches. |
| [SetTopMargin(double value)](./settopmargin/) | Represents the size of the top margin, in unit of centimeters. |
| [SetTopMarginInch(double value)](./settopmargininch/) | Represents the size of the top margin, in unit of inches. |
| [SetZoom(int32_t value)](./setzoom/) | Represents the scaling factor in percent. It should be between 10 and 400. |
| [~PageSetup()](./~pagesetup/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
WorksheetCollection sheets = workbook.GetWorksheets();
//Add a worksheet
sheets.Add();
Worksheet sheet = sheets.Get(1);
PageSetup pageSetup = sheet.GetPageSetup();
pageSetup.SetPrintArea(u"D1:K13");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
