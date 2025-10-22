##PageSetup
Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.
## PageSetup class
Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.
```javascript
class PageSetup;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
sheet.pageSetup.printArea = "D1:K13";
sheet.pageSetup.printTitleRows = "$5:$7";
sheet.pageSetup.printTitleColumns = "$A:$B";
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [oDSPageBackground](#oDSPageBackground--)| OdsPageBackground | Readonly. Gets the background of ODS. |
| [printArea](#printArea--)| string | Represents the range to be printed. |
| [printTitleColumns](#printTitleColumns--)| string | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [printTitleRows](#printTitleRows--)| string | Represents the rows that contain the cells to be repeated at the top of each page. |
| [blackAndWhite](#blackAndWhite--)| boolean | Represents if elements of the document will be printed in black and white. |
| [centerHorizontally](#centerHorizontally--)| boolean | Represent if the sheet is printed centered horizontally. |
| [centerVertically](#centerVertically--)| boolean | Represent if the sheet is printed centered vertically. |
| [printDraft](#printDraft--)| boolean | Represents if the sheet will be printed without graphics. |
| [footerMargin](#footerMargin--)| number | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [footerMarginInch](#footerMarginInch--)| number | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [headerMargin](#headerMargin--)| number | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [headerMarginInch](#headerMarginInch--)| number | Represents the distance from the top of the page to the header, in unit of inches. |
| [printerSettings](#printerSettings--)| Uint8Array | Gets and sets the settings of the default printer. |
| [leftMargin](#leftMargin--)| number | Represents the size of the left margin, in unit of centimeters. |
| [leftMarginInch](#leftMarginInch--)| number | Represents the size of the left margin, in unit of inches. |
| [rightMargin](#rightMargin--)| number | Represents the size of the right margin, in unit of centimeters. |
| [rightMarginInch](#rightMarginInch--)| number | Represents the size of the right margin, in unit of inches. |
| [topMargin](#topMargin--)| number | Represents the size of the top margin, in unit of centimeters. |
| [topMarginInch](#topMarginInch--)| number | Represents the size of the top margin, in unit of inches. |
| [bottomMargin](#bottomMargin--)| number | Represents the size of the bottom margin, in unit of centimeters. |
| [bottomMarginInch](#bottomMarginInch--)| number | Represents the size of the bottom margin, in unit of inches. |
| [firstPageNumber](#firstPageNumber--)| number | Represents the first page number that will be used when this sheet is printed. |
| [fitToPagesTall](#fitToPagesTall--)| number | Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [fitToPagesWide](#fitToPagesWide--)| number | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [isPercentScale](#isPercentScale--)| boolean | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [order](#order--)| PrintOrderType | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [isAutomaticPaperSize](#isAutomaticPaperSize--)| boolean | Readonly. Indicates whether the paper size is automatic. |
| [paperSize](#paperSize--)| PaperSizeType | Represents the size of the paper. |
| [paperWidth](#paperWidth--)| number | Readonly. Gets the width of the paper in unit of inches, considered page orientation. |
| [paperHeight](#paperHeight--)| number | Readonly. Gets the height of the paper in unit of inches , considered page orientation. |
| [orientation](#orientation--)| PageOrientationType | Represents page print orientation. |
| [printComments](#printComments--)| PrintCommentsType | Represents the way comments are printed with the sheet. |
| [printErrors](#printErrors--)| PrintErrorsType | Specifies the type of print error displayed. |
| [printHeadings](#printHeadings--)| boolean | Represents if row and column headings are printed with this page. |
| [printGridlines](#printGridlines--)| boolean | Represents if cell gridlines are printed on the page. |
| [zoom](#zoom--)| number | Represents the scaling factor in percent. It should be between 10 and 400. |
| [isAutoFirstPageNumber](#isAutoFirstPageNumber--)| boolean | Indicates whether the first the page number is automatically assigned. |
| [printQuality](#printQuality--)| number | Represents the print quality. |
| [printCopies](#printCopies--)| number | Get and sets number of copies to print. |
| [isHFDiffOddEven](#isHFDiffOddEven--)| boolean | True means that the header/footer of the odd pages is different with odd pages. |
| [isHFDiffFirst](#isHFDiffFirst--)| boolean | True means that the header/footer of the first page is different with other pages. |
| [isHFScaleWithDoc](#isHFScaleWithDoc--)| boolean | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [isHFAlignMargins](#isHFAlignMargins--)| boolean | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
## Methods
| Method | Description |
| --- | --- |
| [getODSPageBackground()](#getODSPageBackground--)| <b>@deprecated.</b> Please use the 'oDSPageBackground' property instead. Gets the background of ODS. |
| [getPrintArea()](#getPrintArea--)| <b>@deprecated.</b> Please use the 'printArea' property instead. Represents the range to be printed. |
| [setPrintArea(string)](#setPrintArea-string-)| <b>@deprecated.</b> Please use the 'printArea' property instead. Represents the range to be printed. |
| [getPrintTitleColumns()](#getPrintTitleColumns--)| <b>@deprecated.</b> Please use the 'printTitleColumns' property instead. Represents the columns that contain the cells to be repeated on the left side of each page. |
| [setPrintTitleColumns(string)](#setPrintTitleColumns-string-)| <b>@deprecated.</b> Please use the 'printTitleColumns' property instead. Represents the columns that contain the cells to be repeated on the left side of each page. |
| [getPrintTitleRows()](#getPrintTitleRows--)| <b>@deprecated.</b> Please use the 'printTitleRows' property instead. Represents the rows that contain the cells to be repeated at the top of each page. |
| [setPrintTitleRows(string)](#setPrintTitleRows-string-)| <b>@deprecated.</b> Please use the 'printTitleRows' property instead. Represents the rows that contain the cells to be repeated at the top of each page. |
| [getBlackAndWhite()](#getBlackAndWhite--)| <b>@deprecated.</b> Please use the 'blackAndWhite' property instead. Represents if elements of the document will be printed in black and white. |
| [setBlackAndWhite(boolean)](#setBlackAndWhite-boolean-)| <b>@deprecated.</b> Please use the 'blackAndWhite' property instead. Represents if elements of the document will be printed in black and white. |
| [getCenterHorizontally()](#getCenterHorizontally--)| <b>@deprecated.</b> Please use the 'centerHorizontally' property instead. Represent if the sheet is printed centered horizontally. |
| [setCenterHorizontally(boolean)](#setCenterHorizontally-boolean-)| <b>@deprecated.</b> Please use the 'centerHorizontally' property instead. Represent if the sheet is printed centered horizontally. |
| [getCenterVertically()](#getCenterVertically--)| <b>@deprecated.</b> Please use the 'centerVertically' property instead. Represent if the sheet is printed centered vertically. |
| [setCenterVertically(boolean)](#setCenterVertically-boolean-)| <b>@deprecated.</b> Please use the 'centerVertically' property instead. Represent if the sheet is printed centered vertically. |
| [getPrintDraft()](#getPrintDraft--)| <b>@deprecated.</b> Please use the 'printDraft' property instead. Represents if the sheet will be printed without graphics. |
| [setPrintDraft(boolean)](#setPrintDraft-boolean-)| <b>@deprecated.</b> Please use the 'printDraft' property instead. Represents if the sheet will be printed without graphics. |
| [getFooterMargin()](#getFooterMargin--)| <b>@deprecated.</b> Please use the 'footerMargin' property instead. Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [setFooterMargin(number)](#setFooterMargin-number-)| <b>@deprecated.</b> Please use the 'footerMargin' property instead. Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [getFooterMarginInch()](#getFooterMarginInch--)| <b>@deprecated.</b> Please use the 'footerMarginInch' property instead. Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [setFooterMarginInch(number)](#setFooterMarginInch-number-)| <b>@deprecated.</b> Please use the 'footerMarginInch' property instead. Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [getHeaderMargin()](#getHeaderMargin--)| <b>@deprecated.</b> Please use the 'headerMargin' property instead. Represents the distance from the top of the page to the header, in unit of centimeters. |
| [setHeaderMargin(number)](#setHeaderMargin-number-)| <b>@deprecated.</b> Please use the 'headerMargin' property instead. Represents the distance from the top of the page to the header, in unit of centimeters. |
| [getHeaderMarginInch()](#getHeaderMarginInch--)| <b>@deprecated.</b> Please use the 'headerMarginInch' property instead. Represents the distance from the top of the page to the header, in unit of inches. |
| [setHeaderMarginInch(number)](#setHeaderMarginInch-number-)| <b>@deprecated.</b> Please use the 'headerMarginInch' property instead. Represents the distance from the top of the page to the header, in unit of inches. |
| [getPrinterSettings()](#getPrinterSettings--)| <b>@deprecated.</b> Please use the 'printerSettings' property instead. Gets and sets the settings of the default printer. |
| [setPrinterSettings(Uint8Array)](#setPrinterSettings-uint8array-)| <b>@deprecated.</b> Please use the 'printerSettings' property instead. Gets and sets the settings of the default printer. |
| [getLeftMargin()](#getLeftMargin--)| <b>@deprecated.</b> Please use the 'leftMargin' property instead. Represents the size of the left margin, in unit of centimeters. |
| [setLeftMargin(number)](#setLeftMargin-number-)| <b>@deprecated.</b> Please use the 'leftMargin' property instead. Represents the size of the left margin, in unit of centimeters. |
| [getLeftMarginInch()](#getLeftMarginInch--)| <b>@deprecated.</b> Please use the 'leftMarginInch' property instead. Represents the size of the left margin, in unit of inches. |
| [setLeftMarginInch(number)](#setLeftMarginInch-number-)| <b>@deprecated.</b> Please use the 'leftMarginInch' property instead. Represents the size of the left margin, in unit of inches. |
| [getRightMargin()](#getRightMargin--)| <b>@deprecated.</b> Please use the 'rightMargin' property instead. Represents the size of the right margin, in unit of centimeters. |
| [setRightMargin(number)](#setRightMargin-number-)| <b>@deprecated.</b> Please use the 'rightMargin' property instead. Represents the size of the right margin, in unit of centimeters. |
| [getRightMarginInch()](#getRightMarginInch--)| <b>@deprecated.</b> Please use the 'rightMarginInch' property instead. Represents the size of the right margin, in unit of inches. |
| [setRightMarginInch(number)](#setRightMarginInch-number-)| <b>@deprecated.</b> Please use the 'rightMarginInch' property instead. Represents the size of the right margin, in unit of inches. |
| [getTopMargin()](#getTopMargin--)| <b>@deprecated.</b> Please use the 'topMargin' property instead. Represents the size of the top margin, in unit of centimeters. |
| [setTopMargin(number)](#setTopMargin-number-)| <b>@deprecated.</b> Please use the 'topMargin' property instead. Represents the size of the top margin, in unit of centimeters. |
| [getTopMarginInch()](#getTopMarginInch--)| <b>@deprecated.</b> Please use the 'topMarginInch' property instead. Represents the size of the top margin, in unit of inches. |
| [setTopMarginInch(number)](#setTopMarginInch-number-)| <b>@deprecated.</b> Please use the 'topMarginInch' property instead. Represents the size of the top margin, in unit of inches. |
| [getBottomMargin()](#getBottomMargin--)| <b>@deprecated.</b> Please use the 'bottomMargin' property instead. Represents the size of the bottom margin, in unit of centimeters. |
| [setBottomMargin(number)](#setBottomMargin-number-)| <b>@deprecated.</b> Please use the 'bottomMargin' property instead. Represents the size of the bottom margin, in unit of centimeters. |
| [getBottomMarginInch()](#getBottomMarginInch--)| <b>@deprecated.</b> Please use the 'bottomMarginInch' property instead. Represents the size of the bottom margin, in unit of inches. |
| [setBottomMarginInch(number)](#setBottomMarginInch-number-)| <b>@deprecated.</b> Please use the 'bottomMarginInch' property instead. Represents the size of the bottom margin, in unit of inches. |
| [getFirstPageNumber()](#getFirstPageNumber--)| <b>@deprecated.</b> Please use the 'firstPageNumber' property instead. Represents the first page number that will be used when this sheet is printed. |
| [setFirstPageNumber(number)](#setFirstPageNumber-number-)| <b>@deprecated.</b> Please use the 'firstPageNumber' property instead. Represents the first page number that will be used when this sheet is printed. |
| [getFitToPagesTall()](#getFitToPagesTall--)| <b>@deprecated.</b> Please use the 'fitToPagesTall' property instead. Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [setFitToPagesTall(number)](#setFitToPagesTall-number-)| <b>@deprecated.</b> Please use the 'fitToPagesTall' property instead. Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [getFitToPagesWide()](#getFitToPagesWide--)| <b>@deprecated.</b> Please use the 'fitToPagesWide' property instead. Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [setFitToPagesWide(number)](#setFitToPagesWide-number-)| <b>@deprecated.</b> Please use the 'fitToPagesWide' property instead. Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [isPercentScale()](#isPercentScale--)| <b>@deprecated.</b> Please use the 'isPercentScale' property instead. If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [setIsPercentScale(boolean)](#setIsPercentScale-boolean-)| <b>@deprecated.</b> Please use the 'isPercentScale' property instead. If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [getOrder()](#getOrder--)| <b>@deprecated.</b> Please use the 'order' property instead. Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [setOrder(PrintOrderType)](#setOrder-printordertype-)| <b>@deprecated.</b> Please use the 'order' property instead. Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--)| <b>@deprecated.</b> Please use the 'isAutomaticPaperSize' property instead. Indicates whether the paper size is automatic. |
| [getPaperSize()](#getPaperSize--)| <b>@deprecated.</b> Please use the 'paperSize' property instead. Represents the size of the paper. |
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| <b>@deprecated.</b> Please use the 'paperSize' property instead. Represents the size of the paper. |
| [getPaperWidth()](#getPaperWidth--)| <b>@deprecated.</b> Please use the 'paperWidth' property instead. Gets the width of the paper in unit of inches, considered page orientation. |
| [getPaperHeight()](#getPaperHeight--)| <b>@deprecated.</b> Please use the 'paperHeight' property instead. Gets the height of the paper in unit of inches , considered page orientation. |
| [getOrientation()](#getOrientation--)| <b>@deprecated.</b> Please use the 'orientation' property instead. Represents page print orientation. |
| [setOrientation(PageOrientationType)](#setOrientation-pageorientationtype-)| <b>@deprecated.</b> Please use the 'orientation' property instead. Represents page print orientation. |
| [getPrintComments()](#getPrintComments--)| <b>@deprecated.</b> Please use the 'printComments' property instead. Represents the way comments are printed with the sheet. |
| [setPrintComments(PrintCommentsType)](#setPrintComments-printcommentstype-)| <b>@deprecated.</b> Please use the 'printComments' property instead. Represents the way comments are printed with the sheet. |
| [getPrintErrors()](#getPrintErrors--)| <b>@deprecated.</b> Please use the 'printErrors' property instead. Specifies the type of print error displayed. |
| [setPrintErrors(PrintErrorsType)](#setPrintErrors-printerrorstype-)| <b>@deprecated.</b> Please use the 'printErrors' property instead. Specifies the type of print error displayed. |
| [getPrintHeadings()](#getPrintHeadings--)| <b>@deprecated.</b> Please use the 'printHeadings' property instead. Represents if row and column headings are printed with this page. |
| [setPrintHeadings(boolean)](#setPrintHeadings-boolean-)| <b>@deprecated.</b> Please use the 'printHeadings' property instead. Represents if row and column headings are printed with this page. |
| [getPrintGridlines()](#getPrintGridlines--)| <b>@deprecated.</b> Please use the 'printGridlines' property instead. Represents if cell gridlines are printed on the page. |
| [setPrintGridlines(boolean)](#setPrintGridlines-boolean-)| <b>@deprecated.</b> Please use the 'printGridlines' property instead. Represents if cell gridlines are printed on the page. |
| [getZoom()](#getZoom--)| <b>@deprecated.</b> Please use the 'zoom' property instead. Represents the scaling factor in percent. It should be between 10 and 400. |
| [setZoom(number)](#setZoom-number-)| <b>@deprecated.</b> Please use the 'zoom' property instead. Represents the scaling factor in percent. It should be between 10 and 400. |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--)| <b>@deprecated.</b> Please use the 'isAutoFirstPageNumber' property instead. Indicates whether the first the page number is automatically assigned. |
| [setIsAutoFirstPageNumber(boolean)](#setIsAutoFirstPageNumber-boolean-)| <b>@deprecated.</b> Please use the 'isAutoFirstPageNumber' property instead. Indicates whether the first the page number is automatically assigned. |
| [getPrintQuality()](#getPrintQuality--)| <b>@deprecated.</b> Please use the 'printQuality' property instead. Represents the print quality. |
| [setPrintQuality(number)](#setPrintQuality-number-)| <b>@deprecated.</b> Please use the 'printQuality' property instead. Represents the print quality. |
| [getPrintCopies()](#getPrintCopies--)| <b>@deprecated.</b> Please use the 'printCopies' property instead. Get and sets number of copies to print. |
| [setPrintCopies(number)](#setPrintCopies-number-)| <b>@deprecated.</b> Please use the 'printCopies' property instead. Get and sets number of copies to print. |
| [isHFDiffOddEven()](#isHFDiffOddEven--)| <b>@deprecated.</b> Please use the 'isHFDiffOddEven' property instead. True means that the header/footer of the odd pages is different with odd pages. |
| [setIsHFDiffOddEven(boolean)](#setIsHFDiffOddEven-boolean-)| <b>@deprecated.</b> Please use the 'isHFDiffOddEven' property instead. True means that the header/footer of the odd pages is different with odd pages. |
| [isHFDiffFirst()](#isHFDiffFirst--)| <b>@deprecated.</b> Please use the 'isHFDiffFirst' property instead. True means that the header/footer of the first page is different with other pages. |
| [setIsHFDiffFirst(boolean)](#setIsHFDiffFirst-boolean-)| <b>@deprecated.</b> Please use the 'isHFDiffFirst' property instead. True means that the header/footer of the first page is different with other pages. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--)| <b>@deprecated.</b> Please use the 'isHFScaleWithDoc' property instead. Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [setIsHFScaleWithDoc(boolean)](#setIsHFScaleWithDoc-boolean-)| <b>@deprecated.</b> Please use the 'isHFScaleWithDoc' property instead. Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [isHFAlignMargins()](#isHFAlignMargins--)| <b>@deprecated.</b> Please use the 'isHFAlignMargins' property instead. Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
| [setIsHFAlignMargins(boolean)](#setIsHFAlignMargins-boolean-)| <b>@deprecated.</b> Please use the 'isHFAlignMargins' property instead. Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
| [copy(PageSetup, CopyOptions)](#copy-pagesetup-copyoptions-)| Copies the setting of the page setup. |
| [setFitToPages(number, number)](#setFitToPages-number-number-)| Sets the number of pages the worksheet will be scaled to when it's printed. |
| [customPaperSize(number, number)](#customPaperSize-number-number-)| Sets the custom paper size, in unit of inches. |
| [clearHeaderFooter()](#clearHeaderFooter--)| Clears header and footer setting. |
| [getHeader(number)](#getHeader-number-)| Gets a script formatting the header of an Excel file. |
| [getCommands(string)](#getCommands-string-)| Gets all commands of header or footer. |
| [getFooter(number)](#getFooter-number-)| Gets a script formatting the footer of an Excel file. |
| [setHeader(number, string)](#setHeader-number-string-)| Sets a script formatting the header of an Excel file. |
| [setFooter(number, string)](#setFooter-number-string-)| Sets a script formatting the footer of an Excel file. |
| [setEvenHeader(number, string)](#setEvenHeader-number-string-)| Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [getEvenHeader(number)](#getEvenHeader-number-)| Gets a script formatting the even header of an Excel file. |
| [setEvenFooter(number, string)](#setEvenFooter-number-string-)| Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [getEvenFooter(number)](#getEvenFooter-number-)| Gets a script formatting the even footer of an Excel file. |
| [setFirstPageHeader(number, string)](#setFirstPageHeader-number-string-)| Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true. |
| [getFirstPageHeader(number)](#getFirstPageHeader-number-)| Gets a script formatting the first page header of an Excel file. |
| [setFirstPageFooter(number, string)](#setFirstPageFooter-number-string-)| Sets a script formatting the first page footer of an Excel file. |
| [getFirstPageFooter(number)](#getFirstPageFooter-number-)| Gets a script formatting the first page footer of an Excel file. |
| [setHeaderPicture(number, Uint8Array)](#setHeaderPicture-number-uint8array-)| Sets an image in the header of a worksheet. |
| [setFooterPicture(number, Uint8Array)](#setFooterPicture-number-uint8array-)| Sets an image in the footer of a worksheet. |
| [setPicture(boolean, boolean, boolean, number, Uint8Array)](#setPicture-boolean-boolean-boolean-number-uint8array-)| Sets an image in the header/footer of a worksheet. |
| [getPicture(boolean, number)](#getPicture-boolean-number-)| Gets the [Picture](../picture/) object of the header / footer. |
| [getPicture(boolean, boolean, boolean, number)](#getPicture-boolean-boolean-boolean-number-)| Gets the [Picture](../picture/) object of the header / footer. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### oDSPageBackground {#oDSPageBackground--}
Readonly. Gets the background of ODS.
```javascript
oDSPageBackground : OdsPageBackground;
```
### printArea {#printArea--}
Represents the range to be printed.
```javascript
printArea : string;
```
### printTitleColumns {#printTitleColumns--}
Represents the columns that contain the cells to be repeated on the left side of each page.
```javascript
printTitleColumns : string;
```
### printTitleRows {#printTitleRows--}
Represents the rows that contain the cells to be repeated at the top of each page.
```javascript
printTitleRows : string;
```
### blackAndWhite {#blackAndWhite--}
Represents if elements of the document will be printed in black and white.
```javascript
blackAndWhite : boolean;
```
### centerHorizontally {#centerHorizontally--}
Represent if the sheet is printed centered horizontally.
```javascript
centerHorizontally : boolean;
```
### centerVertically {#centerVertically--}
Represent if the sheet is printed centered vertically.
```javascript
centerVertically : boolean;
```
### printDraft {#printDraft--}
Represents if the sheet will be printed without graphics.
```javascript
printDraft : boolean;
```
### footerMargin {#footerMargin--}
Represents the distance from the bottom of the page to the footer, in unit of centimeters.
```javascript
footerMargin : number;
```
### footerMarginInch {#footerMarginInch--}
Represents the distance from the bottom of the page to the footer, in unit of inches.
```javascript
footerMarginInch : number;
```
### headerMargin {#headerMargin--}
Represents the distance from the top of the page to the header, in unit of centimeters.
```javascript
headerMargin : number;
```
### headerMarginInch {#headerMarginInch--}
Represents the distance from the top of the page to the header, in unit of inches.
```javascript
headerMarginInch : number;
```
### printerSettings {#printerSettings--}
Gets and sets the settings of the default printer.
```javascript
printerSettings : Uint8Array;
```
### leftMargin {#leftMargin--}
Represents the size of the left margin, in unit of centimeters.
```javascript
leftMargin : number;
```
### leftMarginInch {#leftMarginInch--}
Represents the size of the left margin, in unit of inches.
```javascript
leftMarginInch : number;
```
### rightMargin {#rightMargin--}
Represents the size of the right margin, in unit of centimeters.
```javascript
rightMargin : number;
```
### rightMarginInch {#rightMarginInch--}
Represents the size of the right margin, in unit of inches.
```javascript
rightMarginInch : number;
```
### topMargin {#topMargin--}
Represents the size of the top margin, in unit of centimeters.
```javascript
topMargin : number;
```
### topMarginInch {#topMarginInch--}
Represents the size of the top margin, in unit of inches.
```javascript
topMarginInch : number;
```
### bottomMargin {#bottomMargin--}
Represents the size of the bottom margin, in unit of centimeters.
```javascript
bottomMargin : number;
```
### bottomMarginInch {#bottomMarginInch--}
Represents the size of the bottom margin, in unit of inches.
```javascript
bottomMarginInch : number;
```
### firstPageNumber {#firstPageNumber--}
Represents the first page number that will be used when this sheet is printed.
```javascript
firstPageNumber : number;
```
### fitToPagesTall {#fitToPagesTall--}
Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1.
```javascript
fitToPagesTall : number;
```
**Remarks**
You have to set FitToPagesWide as zero if you want to fit all rows on one page.
### fitToPagesWide {#fitToPagesWide--}
Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1.
```javascript
fitToPagesWide : number;
```
**Remarks**
You have to set FitToPagesTall as zero if you want to fit all columns on one page.
### isPercentScale {#isPercentScale--}
If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.
```javascript
isPercentScale : boolean;
```
### order {#order--}
Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.
```javascript
order : PrintOrderType;
```
### isAutomaticPaperSize {#isAutomaticPaperSize--}
Readonly. Indicates whether the paper size is automatic.
```javascript
isAutomaticPaperSize : boolean;
```
### paperSize {#paperSize--}
Represents the size of the paper.
```javascript
paperSize : PaperSizeType;
```
### paperWidth {#paperWidth--}
Readonly. Gets the width of the paper in unit of inches, considered page orientation.
```javascript
paperWidth : number;
```
### paperHeight {#paperHeight--}
Readonly. Gets the height of the paper in unit of inches , considered page orientation.
```javascript
paperHeight : number;
```
### orientation {#orientation--}
Represents page print orientation.
```javascript
orientation : PageOrientationType;
```
### printComments {#printComments--}
Represents the way comments are printed with the sheet.
```javascript
printComments : PrintCommentsType;
```
### printErrors {#printErrors--}
Specifies the type of print error displayed.
```javascript
printErrors : PrintErrorsType;
```
### printHeadings {#printHeadings--}
Represents if row and column headings are printed with this page.
```javascript
printHeadings : boolean;
```
### printGridlines {#printGridlines--}
Represents if cell gridlines are printed on the page.
```javascript
printGridlines : boolean;
```
### zoom {#zoom--}
Represents the scaling factor in percent. It should be between 10 and 400.
```javascript
zoom : number;
```
### isAutoFirstPageNumber {#isAutoFirstPageNumber--}
Indicates whether the first the page number is automatically assigned.
```javascript
isAutoFirstPageNumber : boolean;
```
### printQuality {#printQuality--}
Represents the print quality.
```javascript
printQuality : number;
```
### printCopies {#printCopies--}
Get and sets number of copies to print.
```javascript
printCopies : number;
```
### isHFDiffOddEven {#isHFDiffOddEven--}
True means that the header/footer of the odd pages is different with odd pages.
```javascript
isHFDiffOddEven : boolean;
```
### isHFDiffFirst {#isHFDiffFirst--}
True means that the header/footer of the first page is different with other pages.
```javascript
isHFDiffFirst : boolean;
```
### isHFScaleWithDoc {#isHFScaleWithDoc--}
Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.
```javascript
isHFScaleWithDoc : boolean;
```
### isHFAlignMargins {#isHFAlignMargins--}
Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.
```javascript
isHFAlignMargins : boolean;
```
### getODSPageBackground() {#getODSPageBackground--}
```javascript
getODSPageBackground() : OdsPageBackground;
```
**Returns**
[OdsPageBackground](../odspagebackground/)
### getPrintArea() {#getPrintArea--}
```javascript
getPrintArea() : string;
```
### setPrintArea(string) {#setPrintArea-string-}
```javascript
setPrintArea(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getPrintTitleColumns() {#getPrintTitleColumns--}
```javascript
getPrintTitleColumns() : string;
```
### setPrintTitleColumns(string) {#setPrintTitleColumns-string-}
```javascript
setPrintTitleColumns(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getPrintTitleRows() {#getPrintTitleRows--}
```javascript
getPrintTitleRows() : string;
```
### setPrintTitleRows(string) {#setPrintTitleRows-string-}
```javascript
setPrintTitleRows(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getBlackAndWhite() {#getBlackAndWhite--}
```javascript
getBlackAndWhite() : boolean;
```
### setBlackAndWhite(boolean) {#setBlackAndWhite-boolean-}
```javascript
setBlackAndWhite(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCenterHorizontally() {#getCenterHorizontally--}
```javascript
getCenterHorizontally() : boolean;
```
### setCenterHorizontally(boolean) {#setCenterHorizontally-boolean-}
```javascript
setCenterHorizontally(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCenterVertically() {#getCenterVertically--}
```javascript
getCenterVertically() : boolean;
```
### setCenterVertically(boolean) {#setCenterVertically-boolean-}
```javascript
setCenterVertically(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPrintDraft() {#getPrintDraft--}
```javascript
getPrintDraft() : boolean;
```
### setPrintDraft(boolean) {#setPrintDraft-boolean-}
```javascript
setPrintDraft(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFooterMargin() {#getFooterMargin--}
```javascript
getFooterMargin() : number;
```
### setFooterMargin(number) {#setFooterMargin-number-}
```javascript
setFooterMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFooterMarginInch() {#getFooterMarginInch--}
```javascript
getFooterMarginInch() : number;
```
### setFooterMarginInch(number) {#setFooterMarginInch-number-}
```javascript
setFooterMarginInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeaderMargin() {#getHeaderMargin--}
```javascript
getHeaderMargin() : number;
```
### setHeaderMargin(number) {#setHeaderMargin-number-}
```javascript
setHeaderMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeaderMarginInch() {#getHeaderMarginInch--}
```javascript
getHeaderMarginInch() : number;
```
### setHeaderMarginInch(number) {#setHeaderMarginInch-number-}
```javascript
setHeaderMarginInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getPrinterSettings() {#getPrinterSettings--}
```javascript
getPrinterSettings() : Uint8Array;
```
### setPrinterSettings(Uint8Array) {#setPrinterSettings-uint8array-}
```javascript
setPrinterSettings(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getLeftMargin() {#getLeftMargin--}
```javascript
getLeftMargin() : number;
```
### setLeftMargin(number) {#setLeftMargin-number-}
```javascript
setLeftMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLeftMarginInch() {#getLeftMarginInch--}
```javascript
getLeftMarginInch() : number;
```
### setLeftMarginInch(number) {#setLeftMarginInch-number-}
```javascript
setLeftMarginInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRightMargin() {#getRightMargin--}
```javascript
getRightMargin() : number;
```
### setRightMargin(number) {#setRightMargin-number-}
```javascript
setRightMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRightMarginInch() {#getRightMarginInch--}
```javascript
getRightMarginInch() : number;
```
### setRightMarginInch(number) {#setRightMarginInch-number-}
```javascript
setRightMarginInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTopMargin() {#getTopMargin--}
```javascript
getTopMargin() : number;
```
### setTopMargin(number) {#setTopMargin-number-}
```javascript
setTopMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTopMarginInch() {#getTopMarginInch--}
```javascript
getTopMarginInch() : number;
```
### setTopMarginInch(number) {#setTopMarginInch-number-}
```javascript
setTopMarginInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBottomMargin() {#getBottomMargin--}
```javascript
getBottomMargin() : number;
```
### setBottomMargin(number) {#setBottomMargin-number-}
```javascript
setBottomMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBottomMarginInch() {#getBottomMarginInch--}
```javascript
getBottomMarginInch() : number;
```
### setBottomMarginInch(number) {#setBottomMarginInch-number-}
```javascript
setBottomMarginInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFirstPageNumber() {#getFirstPageNumber--}
```javascript
getFirstPageNumber() : number;
```
### setFirstPageNumber(number) {#setFirstPageNumber-number-}
```javascript
setFirstPageNumber(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFitToPagesTall() {#getFitToPagesTall--}
```javascript
getFitToPagesTall() : number;
```
**Remarks**
You have to set FitToPagesWide as zero if you want to fit all rows on one page.
### setFitToPagesTall(number) {#setFitToPagesTall-number-}
```javascript
setFitToPagesTall(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
You have to set FitToPagesWide as zero if you want to fit all rows on one page.
### getFitToPagesWide() {#getFitToPagesWide--}
```javascript
getFitToPagesWide() : number;
```
**Remarks**
You have to set FitToPagesTall as zero if you want to fit all columns on one page.
### setFitToPagesWide(number) {#setFitToPagesWide-number-}
```javascript
setFitToPagesWide(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
You have to set FitToPagesTall as zero if you want to fit all columns on one page.
### isPercentScale() {#isPercentScale--}
```javascript
isPercentScale() : boolean;
```
### setIsPercentScale(boolean) {#setIsPercentScale-boolean-}
```javascript
setIsPercentScale(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getOrder() {#getOrder--}
```javascript
getOrder() : PrintOrderType;
```
**Returns**
[PrintOrderType](../printordertype/)
### setOrder(PrintOrderType) {#setOrder-printordertype-}
```javascript
setOrder(value: PrintOrderType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintOrderType](../printordertype/) | The value to set. |
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```javascript
isAutomaticPaperSize() : boolean;
```
### getPaperSize() {#getPaperSize--}
```javascript
getPaperSize() : PaperSizeType;
```
**Returns**
[PaperSizeType](../papersizetype/)
### setPaperSize(PaperSizeType) {#setPaperSize-papersizetype-}
```javascript
setPaperSize(value: PaperSizeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PaperSizeType](../papersizetype/) | The value to set. |
### getPaperWidth() {#getPaperWidth--}
```javascript
getPaperWidth() : number;
```
### getPaperHeight() {#getPaperHeight--}
```javascript
getPaperHeight() : number;
```
### getOrientation() {#getOrientation--}
```javascript
getOrientation() : PageOrientationType;
```
**Returns**
[PageOrientationType](../pageorientationtype/)
### setOrientation(PageOrientationType) {#setOrientation-pageorientationtype-}
```javascript
setOrientation(value: PageOrientationType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PageOrientationType](../pageorientationtype/) | The value to set. |
### getPrintComments() {#getPrintComments--}
```javascript
getPrintComments() : PrintCommentsType;
```
**Returns**
[PrintCommentsType](../printcommentstype/)
### setPrintComments(PrintCommentsType) {#setPrintComments-printcommentstype-}
```javascript
setPrintComments(value: PrintCommentsType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintCommentsType](../printcommentstype/) | The value to set. |
### getPrintErrors() {#getPrintErrors--}
```javascript
getPrintErrors() : PrintErrorsType;
```
**Returns**
[PrintErrorsType](../printerrorstype/)
### setPrintErrors(PrintErrorsType) {#setPrintErrors-printerrorstype-}
```javascript
setPrintErrors(value: PrintErrorsType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintErrorsType](../printerrorstype/) | The value to set. |
### getPrintHeadings() {#getPrintHeadings--}
```javascript
getPrintHeadings() : boolean;
```
### setPrintHeadings(boolean) {#setPrintHeadings-boolean-}
```javascript
setPrintHeadings(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPrintGridlines() {#getPrintGridlines--}
```javascript
getPrintGridlines() : boolean;
```
### setPrintGridlines(boolean) {#setPrintGridlines-boolean-}
```javascript
setPrintGridlines(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getZoom() {#getZoom--}
```javascript
getZoom() : number;
```
### setZoom(number) {#setZoom-number-}
```javascript
setZoom(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```javascript
isAutoFirstPageNumber() : boolean;
```
### setIsAutoFirstPageNumber(boolean) {#setIsAutoFirstPageNumber-boolean-}
```javascript
setIsAutoFirstPageNumber(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPrintQuality() {#getPrintQuality--}
```javascript
getPrintQuality() : number;
```
### setPrintQuality(number) {#setPrintQuality-number-}
```javascript
setPrintQuality(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getPrintCopies() {#getPrintCopies--}
```javascript
getPrintCopies() : number;
```
### setPrintCopies(number) {#setPrintCopies-number-}
```javascript
setPrintCopies(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isHFDiffOddEven() {#isHFDiffOddEven--}
```javascript
isHFDiffOddEven() : boolean;
```
### setIsHFDiffOddEven(boolean) {#setIsHFDiffOddEven-boolean-}
```javascript
setIsHFDiffOddEven(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isHFDiffFirst() {#isHFDiffFirst--}
```javascript
isHFDiffFirst() : boolean;
```
### setIsHFDiffFirst(boolean) {#setIsHFDiffFirst-boolean-}
```javascript
setIsHFDiffFirst(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```javascript
isHFScaleWithDoc() : boolean;
```
### setIsHFScaleWithDoc(boolean) {#setIsHFScaleWithDoc-boolean-}
```javascript
setIsHFScaleWithDoc(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isHFAlignMargins() {#isHFAlignMargins--}
```javascript
isHFAlignMargins() : boolean;
```
### setIsHFAlignMargins(boolean) {#setIsHFAlignMargins-boolean-}
```javascript
setIsHFAlignMargins(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### copy(PageSetup, CopyOptions) {#copy-pagesetup-copyoptions-}
Copies the setting of the page setup.
```javascript
copy(source: PageSetup, copyOptions: CopyOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [PageSetup](../pagesetup/) | The source. |
| copyOptions | [CopyOptions](../copyoptions/) | The copy options. |
### setFitToPages(number, number) {#setFitToPages-number-number-}
Sets the number of pages the worksheet will be scaled to when it's printed.
```javascript
setFitToPages(wide: number, tall: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wide | number | Pages wide. |
| tall | number | Pages tall. |
### customPaperSize(number, number) {#customPaperSize-number-number-}
Sets the custom paper size, in unit of inches.
```javascript
customPaperSize(width: number, height: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| width | number | The width of the paper. |
| height | number | The height of the paper. |
### clearHeaderFooter() {#clearHeaderFooter--}
Clears header and footer setting.
```javascript
clearHeaderFooter() : void;
```
### getHeader(number) {#getHeader-number-}
Gets a script formatting the header of an Excel file.
```javascript
getHeader(section: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
### getCommands(string) {#getCommands-string-}
Gets all commands of header or footer.
```javascript
getCommands(headerFooterScript: string) : HeaderFooterCommand[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| headerFooterScript | string | The header/footer script |
**Returns**
Returns all commands of header or footer.
### getFooter(number) {#getFooter-number-}
Gets a script formatting the footer of an Excel file.
```javascript
getFooter(section: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
### setHeader(number, string) {#setHeader-number-string-}
Sets a script formatting the header of an Excel file.
```javascript
setHeader(section: number, headerScript: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | string | Header format script. |
**Remarks**
Script commands:</p> <list type="table"> <listheader> <description>Command</description> <description>Description</description> </listheader> <item> <description>&amp;P</description> <description>Current page number　</description> </item> <item> <description>&amp;N</description> <description>Page count　</description> </item> <item> <description>&amp;D</description> <description>Current date　</description> </item> <item> <description>&amp;T</description> <description>Current time</description> </item> <item> <description>&amp;A</description> <description>Sheet name</description> </item> <item> <description>&amp;F</description> <description>File name without path</description> </item> <item> <description>&amp;"&lt;FontName&gt;"</description> <description>Font name, for example: &amp;"Arial"</description> </item> <item> <description>&amp;"&lt;FontName&gt;, &lt;FontStyle&gt;"</description> <description>Font name and font style, for example: &amp;"Arial,Bold"</description> </item> <item> <description>&amp;&lt;FontSize&gt;</description> <description>Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.</description> </item> <item> <description>&amp;K&lt;RRGGBB&gt;</description> <description>Font color, for example(RED): &amp;KFF0000</description> </item> <item> <description>&amp;G</description> <description>Image script</description> </item> </list> For example: "&amp;Arial,Bold&amp;8Header Note"
### setFooter(number, string) {#setFooter-number-string-}
Sets a script formatting the footer of an Excel file.
```javascript
setFooter(section: number, footerScript: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | string | Footer format script. |
**Remarks**
Script commands:</p> <list type="table"> <listheader> <description>Command</description> <description>Description</description> </listheader> <item> <description>&amp;P</description> <description>Current page number　</description> </item> <item> <description>&amp;N</description> <description>Page count　</description> </item> <item> <description>&amp;D</description> <description>Current date　</description> </item> <item> <description>&amp;T</description> <description>Current time</description> </item> <item> <description>&amp;A</description> <description>Sheet name</description> </item> <item> <description>&amp;F</description> <description>File name without path</description> </item> <item> <description>&amp;"&lt;FontName&gt;"</description> <description>Font name, for example: &amp;"Arial"</description> </item> <item> <description>&amp;"&lt;FontName&gt;, &lt;FontStyle&gt;"</description> <description>Font name and font style, for example: &amp;"Arial,Bold"</description> </item> <item> <description>&amp;&lt;FontSize&gt;</description> <description>Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.</description> </item> <item> <description>&amp;K&lt;RRGGBB&gt;</description> <description>Font color, for example(RED): &amp;KFF0000</description> </item> <item> <description>&amp;G</description> <description>Image script</description> </item> </list> For example: "&amp;Arial,Bold&amp;8Footer Note"
### setEvenHeader(number, string) {#setEvenHeader-number-string-}
Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.
```javascript
setEvenHeader(section: number, headerScript: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | string | Header format script. |
### getEvenHeader(number) {#getEvenHeader-number-}
Gets a script formatting the even header of an Excel file.
```javascript
getEvenHeader(section: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
### setEvenFooter(number, string) {#setEvenFooter-number-string-}
Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.
```javascript
setEvenFooter(section: number, footerScript: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | string | Footer format script. |
### getEvenFooter(number) {#getEvenFooter-number-}
Gets a script formatting the even footer of an Excel file.
```javascript
getEvenFooter(section: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
### setFirstPageHeader(number, string) {#setFirstPageHeader-number-string-}
Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true.
```javascript
setFirstPageHeader(section: number, headerScript: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | string | Header format script. |
### getFirstPageHeader(number) {#getFirstPageHeader-number-}
Gets a script formatting the first page header of an Excel file.
```javascript
getFirstPageHeader(section: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
### setFirstPageFooter(number, string) {#setFirstPageFooter-number-string-}
Sets a script formatting the first page footer of an Excel file.
```javascript
setFirstPageFooter(section: number, footerScript: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | string | Footer format script. |
### getFirstPageFooter(number) {#getFirstPageFooter-number-}
Gets a script formatting the first page footer of an Excel file.
```javascript
getFirstPageFooter(section: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
### setHeaderPicture(number, Uint8Array) {#setHeaderPicture-number-uint8array-}
Sets an image in the header of a worksheet.
```javascript
setHeaderPicture(section: number, headerPicture: Uint8Array) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerPicture | number[] | Image data. |
**Returns**
Returns [Picture](../picture/) object.
### setFooterPicture(number, Uint8Array) {#setFooterPicture-number-uint8array-}
Sets an image in the footer of a worksheet.
```javascript
setFooterPicture(section: number, footerPicture: Uint8Array) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerPicture | number[] | Image data. |
**Returns**
Returns [Picture](../picture/) object.
### setPicture(boolean, boolean, boolean, number, Uint8Array) {#setPicture-boolean-boolean-boolean-number-uint8array-}
Sets an image in the header/footer of a worksheet.
```javascript
setPicture(isFirst: boolean, isEven: boolean, isHeader: boolean, section: number, imageData: Uint8Array) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether setting the picture of first page header/footer. |
| isEven | boolean | Indicates whether setting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether setting the picture of header/footer. |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| imageData | number[] | Image data. |
**Returns**
Returns [Picture](../picture/) object.
### getPicture(boolean, number) {#getPicture-boolean-number-}
Gets the [Picture](../picture/) object of the header / footer.
```javascript
getPicture(isHeader: boolean, section: number) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | boolean | Indicates whether it is in the header or footer. |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
**Returns**
Returns [Picture](../picture/) object. Returns null if there is no picture.
### getPicture(boolean, boolean, boolean, number) {#getPicture-boolean-boolean-boolean-number-}
Gets the [Picture](../picture/) object of the header / footer.
```javascript
getPicture(isFirst: boolean, isEven: boolean, isHeader: boolean, section: number) : Picture;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether getting the picture of first page header/footer. |
| isEven | boolean | Indicates whether getting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether getting the picture of header/footer. |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
**Returns**
Returns [Picture](../picture/) object.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
