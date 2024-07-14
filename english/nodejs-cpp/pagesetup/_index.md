---
title: PageSetup
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.
type: docs
url: /nodejs-cpp/pagesetup/
---

## PageSetup class

Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.

```javascript
class PageSetup;
```


## Methods

| Method | Description |
| --- | --- |
| [getODSPageBackground()](#getODSPageBackground--)| Gets the background of ODS. |
| [getPrintArea()](#getPrintArea--)| Represents the range to be printed. |
| [setPrintArea(string)](#setPrintArea-string-)| Represents the range to be printed. |
| [getPrintTitleColumns()](#getPrintTitleColumns--)| Represents the columns that contain the cells to be repeated on the left side of each page. |
| [setPrintTitleColumns(string)](#setPrintTitleColumns-string-)| Represents the columns that contain the cells to be repeated on the left side of each page. |
| [getPrintTitleRows()](#getPrintTitleRows--)| Represents the rows that contain the cells to be repeated at the top of each page. |
| [setPrintTitleRows(string)](#setPrintTitleRows-string-)| Represents the rows that contain the cells to be repeated at the top of each page. |
| [getBlackAndWhite()](#getBlackAndWhite--)| Represents if elements of the document will be printed in black and white. |
| [setBlackAndWhite(boolean)](#setBlackAndWhite-boolean-)| Represents if elements of the document will be printed in black and white. |
| [getCenterHorizontally()](#getCenterHorizontally--)| Represent if the sheet is printed centered horizontally. |
| [setCenterHorizontally(boolean)](#setCenterHorizontally-boolean-)| Represent if the sheet is printed centered horizontally. |
| [getCenterVertically()](#getCenterVertically--)| Represent if the sheet is printed centered vertically. |
| [setCenterVertically(boolean)](#setCenterVertically-boolean-)| Represent if the sheet is printed centered vertically. |
| [getPrintDraft()](#getPrintDraft--)| Represents if the sheet will be printed without graphics. |
| [setPrintDraft(boolean)](#setPrintDraft-boolean-)| Represents if the sheet will be printed without graphics. |
| [getFooterMargin()](#getFooterMargin--)| Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [setFooterMargin(number)](#setFooterMargin-number-)| Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [getFooterMarginInch()](#getFooterMarginInch--)| Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [setFooterMarginInch(number)](#setFooterMarginInch-number-)| Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [getHeaderMargin()](#getHeaderMargin--)| Represents the distance from the top of the page to the header, in unit of centimeters. |
| [setHeaderMargin(number)](#setHeaderMargin-number-)| Represents the distance from the top of the page to the header, in unit of centimeters. |
| [getHeaderMarginInch()](#getHeaderMarginInch--)| Represents the distance from the top of the page to the header, in unit of inches. |
| [setHeaderMarginInch(number)](#setHeaderMarginInch-number-)| Represents the distance from the top of the page to the header, in unit of inches. |
| [getPrinterSettings()](#getPrinterSettings--)| Gets and sets the settings of the default printer. |
| [setPrinterSettings(number[])](#setPrinterSettings-numberarray-)| Gets and sets the settings of the default printer. |
| [getLeftMargin()](#getLeftMargin--)| Represents the size of the left margin, in unit of centimeters. |
| [setLeftMargin(number)](#setLeftMargin-number-)| Represents the size of the left margin, in unit of centimeters. |
| [getLeftMarginInch()](#getLeftMarginInch--)| Represents the size of the left margin, in unit of inches. |
| [setLeftMarginInch(number)](#setLeftMarginInch-number-)| Represents the size of the left margin, in unit of inches. |
| [getRightMargin()](#getRightMargin--)| Represents the size of the right margin, in unit of centimeters. |
| [setRightMargin(number)](#setRightMargin-number-)| Represents the size of the right margin, in unit of centimeters. |
| [getRightMarginInch()](#getRightMarginInch--)| Represents the size of the right margin, in unit of inches. |
| [setRightMarginInch(number)](#setRightMarginInch-number-)| Represents the size of the right margin, in unit of inches. |
| [getTopMargin()](#getTopMargin--)| Represents the size of the top margin, in unit of centimeters. |
| [setTopMargin(number)](#setTopMargin-number-)| Represents the size of the top margin, in unit of centimeters. |
| [getTopMarginInch()](#getTopMarginInch--)| Represents the size of the top margin, in unit of inches. |
| [setTopMarginInch(number)](#setTopMarginInch-number-)| Represents the size of the top margin, in unit of inches. |
| [getBottomMargin()](#getBottomMargin--)| Represents the size of the bottom margin, in unit of centimeters. |
| [setBottomMargin(number)](#setBottomMargin-number-)| Represents the size of the bottom margin, in unit of centimeters. |
| [getBottomMarginInch()](#getBottomMarginInch--)| Represents the size of the bottom margin, in unit of inches. |
| [setBottomMarginInch(number)](#setBottomMarginInch-number-)| Represents the size of the bottom margin, in unit of inches. |
| [getFirstPageNumber()](#getFirstPageNumber--)| Represents the first page number that will be used when this sheet is printed. |
| [setFirstPageNumber(number)](#setFirstPageNumber-number-)| Represents the first page number that will be used when this sheet is printed. |
| [getFitToPagesTall()](#getFitToPagesTall--)| Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [setFitToPagesTall(number)](#setFitToPagesTall-number-)| Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. |
| [getFitToPagesWide()](#getFitToPagesWide--)| Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [setFitToPagesWide(number)](#setFitToPagesWide-number-)| Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. |
| [isPercentScale()](#isPercentScale--)| If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [setIsPercentScale(boolean)](#setIsPercentScale-boolean-)| If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [getOrder()](#getOrder--)| Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [setOrder(PrintOrderType)](#setOrder-printordertype-)| Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--)| Indicates whether the paper size is automatic. |
| [getPaperSize()](#getPaperSize--)| Represents the size of the paper. |
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| Represents the size of the paper. |
| [getPaperWidth()](#getPaperWidth--)| Gets the width of the paper in unit of inches, considered page orientation. |
| [getPaperHeight()](#getPaperHeight--)| Gets the height of the paper in unit of inches , considered page orientation. |
| [getOrientation()](#getOrientation--)| Represents page print orientation. |
| [setOrientation(PageOrientationType)](#setOrientation-pageorientationtype-)| Represents page print orientation. |
| [getPrintComments()](#getPrintComments--)| Represents the way comments are printed with the sheet. |
| [setPrintComments(PrintCommentsType)](#setPrintComments-printcommentstype-)| Represents the way comments are printed with the sheet. |
| [getPrintErrors()](#getPrintErrors--)| Specifies the type of print error displayed. |
| [setPrintErrors(PrintErrorsType)](#setPrintErrors-printerrorstype-)| Specifies the type of print error displayed. |
| [getPrintHeadings()](#getPrintHeadings--)| Represents if row and column headings are printed with this page. |
| [setPrintHeadings(boolean)](#setPrintHeadings-boolean-)| Represents if row and column headings are printed with this page. |
| [getPrintGridlines()](#getPrintGridlines--)| Represents if cell gridlines are printed on the page. |
| [setPrintGridlines(boolean)](#setPrintGridlines-boolean-)| Represents if cell gridlines are printed on the page. |
| [getZoom()](#getZoom--)| Represents the scaling factor in percent. It should be between 10 and 400. |
| [setZoom(number)](#setZoom-number-)| Represents the scaling factor in percent. It should be between 10 and 400. |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--)| Indicates whether the first the page number is automatically assigned. |
| [setIsAutoFirstPageNumber(boolean)](#setIsAutoFirstPageNumber-boolean-)| Indicates whether the first the page number is automatically assigned. |
| [getPrintQuality()](#getPrintQuality--)| Represents the print quality. |
| [setPrintQuality(number)](#setPrintQuality-number-)| Represents the print quality. |
| [getPrintCopies()](#getPrintCopies--)| Get and sets number of copies to print. |
| [setPrintCopies(number)](#setPrintCopies-number-)| Get and sets number of copies to print. |
| [isHFDiffOddEven()](#isHFDiffOddEven--)| True means that the header/footer of the odd pages is different with odd pages. |
| [setIsHFDiffOddEven(boolean)](#setIsHFDiffOddEven-boolean-)| True means that the header/footer of the odd pages is different with odd pages. |
| [isHFDiffFirst()](#isHFDiffFirst--)| True means that the header/footer of the first page is different with other pages. |
| [setIsHFDiffFirst(boolean)](#setIsHFDiffFirst-boolean-)| True means that the header/footer of the first page is different with other pages. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--)| Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [setIsHFScaleWithDoc(boolean)](#setIsHFScaleWithDoc-boolean-)| Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [isHFAlignMargins()](#isHFAlignMargins--)| Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
| [setIsHFAlignMargins(boolean)](#setIsHFAlignMargins-boolean-)| Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default. |
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
| [setHeaderPicture(number, number[])](#setHeaderPicture-number-numberarray-)| Sets an image in the header of a worksheet. |
| [setFooterPicture(number, number[])](#setFooterPicture-number-numberarray-)| Sets an image in the footer of a worksheet. |
| [setPicture(boolean, boolean, boolean, number, number[])](#setPicture-boolean-boolean-boolean-number-numberarray-)| Sets an image in the header/footer of a worksheet. |
| [getPicture(boolean, number)](#getPicture-boolean-number-)| Gets the [Picture](/nodejs-cpp/picture/) object of the header / footer. |
| [getPicture(boolean, boolean, boolean, number)](#getPicture-boolean-boolean-boolean-number-)| Gets the [Picture](/nodejs-cpp/picture/) object of the header / footer. |


### getODSPageBackground() {#getODSPageBackground--}

Gets the background of ODS.

```javascript
getODSPageBackground() : OdsPageBackground;
```


**Returns**

[OdsPageBackground](/nodejs-cpp/odspagebackground/)

### getPrintArea() {#getPrintArea--}

Represents the range to be printed.

```javascript
getPrintArea() : string;
```


### setPrintArea(string) {#setPrintArea-string-}

Represents the range to be printed.

```javascript
setPrintArea(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPrintTitleColumns() {#getPrintTitleColumns--}

Represents the columns that contain the cells to be repeated on the left side of each page.

```javascript
getPrintTitleColumns() : string;
```


### setPrintTitleColumns(string) {#setPrintTitleColumns-string-}

Represents the columns that contain the cells to be repeated on the left side of each page.

```javascript
setPrintTitleColumns(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPrintTitleRows() {#getPrintTitleRows--}

Represents the rows that contain the cells to be repeated at the top of each page.

```javascript
getPrintTitleRows() : string;
```


### setPrintTitleRows(string) {#setPrintTitleRows-string-}

Represents the rows that contain the cells to be repeated at the top of each page.

```javascript
setPrintTitleRows(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getBlackAndWhite() {#getBlackAndWhite--}

Represents if elements of the document will be printed in black and white.

```javascript
getBlackAndWhite() : boolean;
```


### setBlackAndWhite(boolean) {#setBlackAndWhite-boolean-}

Represents if elements of the document will be printed in black and white.

```javascript
setBlackAndWhite(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCenterHorizontally() {#getCenterHorizontally--}

Represent if the sheet is printed centered horizontally.

```javascript
getCenterHorizontally() : boolean;
```


### setCenterHorizontally(boolean) {#setCenterHorizontally-boolean-}

Represent if the sheet is printed centered horizontally.

```javascript
setCenterHorizontally(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCenterVertically() {#getCenterVertically--}

Represent if the sheet is printed centered vertically.

```javascript
getCenterVertically() : boolean;
```


### setCenterVertically(boolean) {#setCenterVertically-boolean-}

Represent if the sheet is printed centered vertically.

```javascript
setCenterVertically(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintDraft() {#getPrintDraft--}

Represents if the sheet will be printed without graphics.

```javascript
getPrintDraft() : boolean;
```


### setPrintDraft(boolean) {#setPrintDraft-boolean-}

Represents if the sheet will be printed without graphics.

```javascript
setPrintDraft(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFooterMargin() {#getFooterMargin--}

Represents the distance from the bottom of the page to the footer, in unit of centimeters.

```javascript
getFooterMargin() : number;
```


### setFooterMargin(number) {#setFooterMargin-number-}

Represents the distance from the bottom of the page to the footer, in unit of centimeters.

```javascript
setFooterMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFooterMarginInch() {#getFooterMarginInch--}

Represents the distance from the bottom of the page to the footer, in unit of inches.

```javascript
getFooterMarginInch() : number;
```


### setFooterMarginInch(number) {#setFooterMarginInch-number-}

Represents the distance from the bottom of the page to the footer, in unit of inches.

```javascript
setFooterMarginInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeaderMargin() {#getHeaderMargin--}

Represents the distance from the top of the page to the header, in unit of centimeters.

```javascript
getHeaderMargin() : number;
```


### setHeaderMargin(number) {#setHeaderMargin-number-}

Represents the distance from the top of the page to the header, in unit of centimeters.

```javascript
setHeaderMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeaderMarginInch() {#getHeaderMarginInch--}

Represents the distance from the top of the page to the header, in unit of inches.

```javascript
getHeaderMarginInch() : number;
```


### setHeaderMarginInch(number) {#setHeaderMarginInch-number-}

Represents the distance from the top of the page to the header, in unit of inches.

```javascript
setHeaderMarginInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPrinterSettings() {#getPrinterSettings--}

Gets and sets the settings of the default printer.

```javascript
getPrinterSettings() : number[];
```


**Returns**

number[]

### setPrinterSettings(number[]) {#setPrinterSettings-numberarray-}

Gets and sets the settings of the default printer.

```javascript
setPrinterSettings(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getLeftMargin() {#getLeftMargin--}

Represents the size of the left margin, in unit of centimeters.

```javascript
getLeftMargin() : number;
```


### setLeftMargin(number) {#setLeftMargin-number-}

Represents the size of the left margin, in unit of centimeters.

```javascript
setLeftMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftMarginInch() {#getLeftMarginInch--}

Represents the size of the left margin, in unit of inches.

```javascript
getLeftMarginInch() : number;
```


### setLeftMarginInch(number) {#setLeftMarginInch-number-}

Represents the size of the left margin, in unit of inches.

```javascript
setLeftMarginInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRightMargin() {#getRightMargin--}

Represents the size of the right margin, in unit of centimeters.

```javascript
getRightMargin() : number;
```


### setRightMargin(number) {#setRightMargin-number-}

Represents the size of the right margin, in unit of centimeters.

```javascript
setRightMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRightMarginInch() {#getRightMarginInch--}

Represents the size of the right margin, in unit of inches.

```javascript
getRightMarginInch() : number;
```


### setRightMarginInch(number) {#setRightMarginInch-number-}

Represents the size of the right margin, in unit of inches.

```javascript
setRightMarginInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopMargin() {#getTopMargin--}

Represents the size of the top margin, in unit of centimeters.

```javascript
getTopMargin() : number;
```


### setTopMargin(number) {#setTopMargin-number-}

Represents the size of the top margin, in unit of centimeters.

```javascript
setTopMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopMarginInch() {#getTopMarginInch--}

Represents the size of the top margin, in unit of inches.

```javascript
getTopMarginInch() : number;
```


### setTopMarginInch(number) {#setTopMarginInch-number-}

Represents the size of the top margin, in unit of inches.

```javascript
setTopMarginInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBottomMargin() {#getBottomMargin--}

Represents the size of the bottom margin, in unit of centimeters.

```javascript
getBottomMargin() : number;
```


### setBottomMargin(number) {#setBottomMargin-number-}

Represents the size of the bottom margin, in unit of centimeters.

```javascript
setBottomMargin(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBottomMarginInch() {#getBottomMarginInch--}

Represents the size of the bottom margin, in unit of inches.

```javascript
getBottomMarginInch() : number;
```


### setBottomMarginInch(number) {#setBottomMarginInch-number-}

Represents the size of the bottom margin, in unit of inches.

```javascript
setBottomMarginInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFirstPageNumber() {#getFirstPageNumber--}

Represents the first page number that will be used when this sheet is printed.

```javascript
getFirstPageNumber() : number;
```


### setFirstPageNumber(number) {#setFirstPageNumber-number-}

Represents the first page number that will be used when this sheet is printed.

```javascript
setFirstPageNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFitToPagesTall() {#getFitToPagesTall--}

Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1.

```javascript
getFitToPagesTall() : number;
```


**Remarks**

You have to set FitToPagesWide as zero if you want to fit all rows on one page.

### setFitToPagesTall(number) {#setFitToPagesTall-number-}

Represents  the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1.

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

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1.

```javascript
getFitToPagesWide() : number;
```


**Remarks**

You have to set FitToPagesTall as zero if you want to fit all columns on one page.

### setFitToPagesWide(number) {#setFitToPagesWide-number-}

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1.

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

If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

```javascript
isPercentScale() : boolean;
```


### setIsPercentScale(boolean) {#setIsPercentScale-boolean-}

If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

```javascript
setIsPercentScale(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOrder() {#getOrder--}

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.

```javascript
getOrder() : PrintOrderType;
```


**Returns**

[PrintOrderType](/nodejs-cpp/printordertype/)

### setOrder(PrintOrderType) {#setOrder-printordertype-}

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.

```javascript
setOrder(value: PrintOrderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintOrderType](/nodejs-cpp/printordertype/) | The value to set. |

### isAutomaticPaperSize() {#isAutomaticPaperSize--}

Indicates whether the paper size is automatic.

```javascript
isAutomaticPaperSize() : boolean;
```


### getPaperSize() {#getPaperSize--}

Represents the size of the paper.

```javascript
getPaperSize() : PaperSizeType;
```


**Returns**

[PaperSizeType](/nodejs-cpp/papersizetype/)

### setPaperSize(PaperSizeType) {#setPaperSize-papersizetype-}

Represents the size of the paper.

```javascript
setPaperSize(value: PaperSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PaperSizeType](/nodejs-cpp/papersizetype/) | The value to set. |

### getPaperWidth() {#getPaperWidth--}

Gets the width of the paper in unit of inches, considered page orientation.

```javascript
getPaperWidth() : number;
```


### getPaperHeight() {#getPaperHeight--}

Gets the height of the paper in unit of inches , considered page orientation.

```javascript
getPaperHeight() : number;
```


### getOrientation() {#getOrientation--}

Represents page print orientation.

```javascript
getOrientation() : PageOrientationType;
```


**Returns**

[PageOrientationType](/nodejs-cpp/pageorientationtype/)

### setOrientation(PageOrientationType) {#setOrientation-pageorientationtype-}

Represents page print orientation.

```javascript
setOrientation(value: PageOrientationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PageOrientationType](/nodejs-cpp/pageorientationtype/) | The value to set. |

### getPrintComments() {#getPrintComments--}

Represents the way comments are printed with the sheet.

```javascript
getPrintComments() : PrintCommentsType;
```


**Returns**

[PrintCommentsType](/nodejs-cpp/printcommentstype/)

### setPrintComments(PrintCommentsType) {#setPrintComments-printcommentstype-}

Represents the way comments are printed with the sheet.

```javascript
setPrintComments(value: PrintCommentsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintCommentsType](/nodejs-cpp/printcommentstype/) | The value to set. |

### getPrintErrors() {#getPrintErrors--}

Specifies the type of print error displayed.

```javascript
getPrintErrors() : PrintErrorsType;
```


**Returns**

[PrintErrorsType](/nodejs-cpp/printerrorstype/)

### setPrintErrors(PrintErrorsType) {#setPrintErrors-printerrorstype-}

Specifies the type of print error displayed.

```javascript
setPrintErrors(value: PrintErrorsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintErrorsType](/nodejs-cpp/printerrorstype/) | The value to set. |

### getPrintHeadings() {#getPrintHeadings--}

Represents if row and column headings are printed with this page.

```javascript
getPrintHeadings() : boolean;
```


### setPrintHeadings(boolean) {#setPrintHeadings-boolean-}

Represents if row and column headings are printed with this page.

```javascript
setPrintHeadings(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintGridlines() {#getPrintGridlines--}

Represents if cell gridlines are printed on the page.

```javascript
getPrintGridlines() : boolean;
```


### setPrintGridlines(boolean) {#setPrintGridlines-boolean-}

Represents if cell gridlines are printed on the page.

```javascript
setPrintGridlines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getZoom() {#getZoom--}

Represents the scaling factor in percent. It should be between 10 and 400.

```javascript
getZoom() : number;
```


### setZoom(number) {#setZoom-number-}

Represents the scaling factor in percent. It should be between 10 and 400.

```javascript
setZoom(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}

Indicates whether the first the page number is automatically assigned.

```javascript
isAutoFirstPageNumber() : boolean;
```


### setIsAutoFirstPageNumber(boolean) {#setIsAutoFirstPageNumber-boolean-}

Indicates whether the first the page number is automatically assigned.

```javascript
setIsAutoFirstPageNumber(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintQuality() {#getPrintQuality--}

Represents the print quality.

```javascript
getPrintQuality() : number;
```


### setPrintQuality(number) {#setPrintQuality-number-}

Represents the print quality.

```javascript
setPrintQuality(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPrintCopies() {#getPrintCopies--}

Get and sets number of copies to print.

```javascript
getPrintCopies() : number;
```


### setPrintCopies(number) {#setPrintCopies-number-}

Get and sets number of copies to print.

```javascript
setPrintCopies(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isHFDiffOddEven() {#isHFDiffOddEven--}

True means that the header/footer of the odd pages is different with odd pages.

```javascript
isHFDiffOddEven() : boolean;
```


### setIsHFDiffOddEven(boolean) {#setIsHFDiffOddEven-boolean-}

True means that the header/footer of the odd pages is different with odd pages.

```javascript
setIsHFDiffOddEven(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHFDiffFirst() {#isHFDiffFirst--}

True means that the header/footer of the first page is different with other pages.

```javascript
isHFDiffFirst() : boolean;
```


### setIsHFDiffFirst(boolean) {#setIsHFDiffFirst-boolean-}

True means that the header/footer of the first page is different with other pages.

```javascript
setIsHFDiffFirst(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHFScaleWithDoc() {#isHFScaleWithDoc--}

Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

```javascript
isHFScaleWithDoc() : boolean;
```


### setIsHFScaleWithDoc(boolean) {#setIsHFScaleWithDoc-boolean-}

Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

```javascript
setIsHFScaleWithDoc(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHFAlignMargins() {#isHFAlignMargins--}

Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

```javascript
isHFAlignMargins() : boolean;
```


### setIsHFAlignMargins(boolean) {#setIsHFAlignMargins-boolean-}

Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

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
| source | [PageSetup](/nodejs-cpp/pagesetup/) | The source. |
| copyOptions | [CopyOptions](/nodejs-cpp/copyoptions/) | The copy options. |

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

<p>Script commands:</p> <list type="table"> <listheader> <description>Command</description> <description>Description</description> </listheader> <item> <description>&amp;P</description> <description>Current page number　</description> </item> <item> <description>&amp;N</description> <description>Page count　</description> </item> <item> <description>&amp;D</description> <description>Current date　</description> </item> <item> <description>&amp;T</description> <description>Current time</description> </item> <item> <description>&amp;A</description> <description>Sheet name</description> </item> <item> <description>&amp;F</description> <description>File name without path</description> </item> <item> <description>&amp;"&lt;FontName&gt;"</description> <description>Font name, for example: &amp;"Arial"</description> </item> <item> <description>&amp;"&lt;FontName&gt;, &lt;FontStyle&gt;"</description> <description>Font name and font style, for example: &amp;"Arial,Bold"</description> </item> <item> <description>&amp;&lt;FontSize&gt;</description> <description>Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.</description> </item> <item> <description>&amp;K&lt;RRGGBB&gt;</description> <description>Font color, for example(RED): &amp;KFF0000</description> </item> <item> <description>&amp;G</description> <description>Image script</description> </item> </list> For example: "&amp;Arial,Bold&amp;8Header Note"

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

<p>Script commands:</p> <list type="table"> <listheader> <description>Command</description> <description>Description</description> </listheader> <item> <description>&amp;P</description> <description>Current page number　</description> </item> <item> <description>&amp;N</description> <description>Page count　</description> </item> <item> <description>&amp;D</description> <description>Current date　</description> </item> <item> <description>&amp;T</description> <description>Current time</description> </item> <item> <description>&amp;A</description> <description>Sheet name</description> </item> <item> <description>&amp;F</description> <description>File name without path</description> </item> <item> <description>&amp;"&lt;FontName&gt;"</description> <description>Font name, for example: &amp;"Arial"</description> </item> <item> <description>&amp;"&lt;FontName&gt;, &lt;FontStyle&gt;"</description> <description>Font name and font style, for example: &amp;"Arial,Bold"</description> </item> <item> <description>&amp;&lt;FontSize&gt;</description> <description>Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.</description> </item> <item> <description>&amp;K&lt;RRGGBB&gt;</description> <description>Font color, for example(RED): &amp;KFF0000</description> </item> <item> <description>&amp;G</description> <description>Image script</description> </item> </list> For example: "&amp;Arial,Bold&amp;8Footer Note"

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

### setHeaderPicture(number, number[]) {#setHeaderPicture-number-numberarray-}

Sets an image in the header of a worksheet.

```javascript
setHeaderPicture(section: number, headerPicture: number[]) : Picture;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerPicture | number[] | Image data. |

**Returns**

Returns [Picture](/nodejs-cpp/picture/) object.

### setFooterPicture(number, number[]) {#setFooterPicture-number-numberarray-}

Sets an image in the footer of a worksheet.

```javascript
setFooterPicture(section: number, footerPicture: number[]) : Picture;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerPicture | number[] | Image data. |

**Returns**

Returns [Picture](/nodejs-cpp/picture/) object.

### setPicture(boolean, boolean, boolean, number, number[]) {#setPicture-boolean-boolean-boolean-number-numberarray-}

Sets an image in the header/footer of a worksheet.

```javascript
setPicture(isFirst: boolean, isEven: boolean, isHeader: boolean, section: number, imageData: number[]) : Picture;
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

Returns [Picture](/nodejs-cpp/picture/) object.

### getPicture(boolean, number) {#getPicture-boolean-number-}

Gets the [Picture](/nodejs-cpp/picture/) object of the header / footer.

```javascript
getPicture(isHeader: boolean, section: number) : Picture;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | boolean | Indicates whether it is in the header or footer. |
| section | number | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns**

Returns [Picture](/nodejs-cpp/picture/) object. Returns null if there is no picture.

### getPicture(boolean, boolean, boolean, number) {#getPicture-boolean-boolean-boolean-number-}

Gets the [Picture](/nodejs-cpp/picture/) object of the header / footer.

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

Returns [Picture](/nodejs-cpp/picture/) object.


