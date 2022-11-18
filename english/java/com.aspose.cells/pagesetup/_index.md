---
title: PageSetup
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents the page setup description.
type: docs
weight: 371
url: /java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.

```
Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## Methods

| Method | Description |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Clears header and footer setting. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Copies the setting of the page setup. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Sets the custom paper size, in unit of inches. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Represents if elements of the document will be printed in black and white. |
| [getBottomMargin()](#getBottomMargin--) | Represents the size of the bottom margin, in unit of centimeters. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Represents the size of the bottom margin, in unit of inches. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Represent if the sheet is printed centered horizontally. |
| [getCenterVertically()](#getCenterVertically--) | Represent if the sheet is printed centered vertically. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Gets all commands of header or footer. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Gets a script formatting the even footer of an Excel file. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Gets a script formatting the even header of an Excel file. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Gets a script formatting the first page footer of an Excel file. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Gets a script formatting the first page header of an Excel file. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Represents the first page number that will be used when this sheet is printed. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Represents the number of pages tall the worksheet will be scaled to when it's printed. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Represents the number of pages wide the worksheet will be scaled to when it's printed. |
| [getFooter(int section)](#getFooter-int-) | Gets a script formatting the footer of an Excel file. |
| [getFooterMargin()](#getFooterMargin--) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [getHeader(int section)](#getHeader-int-) | Gets a script formatting the header of an Excel file. |
| [getHeaderMargin()](#getHeaderMargin--) | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Represents the distance from the top of the page to the header, in unit of inches. |
| [getLeftMargin()](#getLeftMargin--) | Represents the size of the left margin, in unit of centimeters. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Represents the size of the left margin, in unit of inches. |
| [getODSPageBackground()](#getODSPageBackground--) | Gets the background of ODS. |
| [getOrder()](#getOrder--) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. |
| [getOrientation()](#getOrientation--) | Represents page print orientation. |
| [getPaperHeight()](#getPaperHeight--) | Gets the height of the paper in unit of inches , considered page orientation. |
| [getPaperSize()](#getPaperSize--) | Represents the size of the paper. |
| [getPaperWidth()](#getPaperWidth--) | Gets the width of the paper in unit of inches, considered page orientation. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Gets the [Picture](../../com.aspose.cells/picture) object of the header / footer. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Gets the [Picture](../../com.aspose.cells/picture) object of the header / footer. |
| [getPrintArea()](#getPrintArea--) | Represents the range to be printed. |
| [getPrintComments()](#getPrintComments--) | Represents the way comments are printed with the sheet. |
| [getPrintCopies()](#getPrintCopies--) | Get and sets number of copies to print. |
| [getPrintDraft()](#getPrintDraft--) | Represents if the sheet will be printed without graphics. |
| [getPrintErrors()](#getPrintErrors--) | Specifies the type of print error displayed. |
| [getPrintGridlines()](#getPrintGridlines--) | Represents if cell gridlines are printed on the page. |
| [getPrintHeadings()](#getPrintHeadings--) | Represents if row and column headings are printed with this page. |
| [getPrintQuality()](#getPrintQuality--) | Represents the print quality. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [getPrinterSettings()](#getPrinterSettings--) | Gets and sets the settings of the default printer. |
| [getRightMargin()](#getRightMargin--) | Represents the size of the right margin, in unit of centimeters. |
| [getRightMarginInch()](#getRightMarginInch--) | Represents the size of the right margin, in unit of inches. |
| [getTopMargin()](#getTopMargin--) | Represents the size of the top margin, in unit of centimeters. |
| [getTopMarginInch()](#getTopMarginInch--) | Represents the size of the top margin, in unit of inches. |
| [getZoom()](#getZoom--) | Represents the scaling factor in percent. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Indicates whether the first the page number is automatically assigned. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Indicates whether the paper size is automatic. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Indicates whether header and footer margins are aligned with the page margins. |
| [isHFDiffFirst()](#isHFDiffFirst--) | True means that the header/footer of the first page is different with other pages. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | True means that the header/footer of the odd pages is different with odd pages. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Indicates whether header and footer are scaled with document scaling. |
| [isPercentScale()](#isPercentScale--) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Please see the getter of this property: [isAutoFirstPageNumber()](../../com.aspose.cells/pagesetup\#isAutoFirstPageNumber--) |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Please see the getter of this property: [getBlackAndWhite()](../../com.aspose.cells/pagesetup\#getBlackAndWhite--) |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Please see the getter of this property: [getBottomMargin()](../../com.aspose.cells/pagesetup\#getBottomMargin--) |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Please see the getter of this property: [getBottomMarginInch()](../../com.aspose.cells/pagesetup\#getBottomMarginInch--) |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Please see the getter of this property: [getCenterHorizontally()](../../com.aspose.cells/pagesetup\#getCenterHorizontally--) |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Please see the getter of this property: [getCenterVertically()](../../com.aspose.cells/pagesetup\#getCenterVertically--) |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Sets a script formatting the even page footer of an Excel file. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Sets a script formatting the even page header of an Excel file. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Sets a script formatting the first page footer of an Excel file. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Sets a script formatting the first page header of an Excel file. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Please see the getter of this property: [getFirstPageNumber()](../../com.aspose.cells/pagesetup\#getFirstPageNumber--) |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Sets the number of pages the worksheet will be scaled to when it's printed. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Please see the getter of this property: [getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--) |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Please see the getter of this property: [getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Sets a script formatting the footer of an Excel file. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Please see the getter of this property: [getFooterMargin()](../../com.aspose.cells/pagesetup\#getFooterMargin--) |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Please see the getter of this property: [getFooterMarginInch()](../../com.aspose.cells/pagesetup\#getFooterMarginInch--) |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Sets an image in the footer of a worksheet. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Please see the getter of this property: [isHFAlignMargins()](../../com.aspose.cells/pagesetup\#isHFAlignMargins--) |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | Please see the getter of this property: [isHFDiffFirst()](../../com.aspose.cells/pagesetup\#isHFDiffFirst--) |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | Please see the getter of this property: [isHFDiffOddEven()](../../com.aspose.cells/pagesetup\#isHFDiffOddEven--) |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Please see the getter of this property: [isHFScaleWithDoc()](../../com.aspose.cells/pagesetup\#isHFScaleWithDoc--) |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Sets a script formatting the header of an Excel file. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Please see the getter of this property: [getHeaderMargin()](../../com.aspose.cells/pagesetup\#getHeaderMargin--) |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Please see the getter of this property: [getHeaderMarginInch()](../../com.aspose.cells/pagesetup\#getHeaderMarginInch--) |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Sets an image in the header of a worksheet. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Please see the getter of this property: [getLeftMargin()](../../com.aspose.cells/pagesetup\#getLeftMargin--) |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Please see the getter of this property: [getLeftMarginInch()](../../com.aspose.cells/pagesetup\#getLeftMarginInch--) |
| [setOrder(int value)](#setOrder-int-) | Please see the getter of this property: [getOrder()](../../com.aspose.cells/pagesetup\#getOrder--) |
| [setOrientation(int value)](#setOrientation-int-) | Please see the getter of this property: [getOrientation()](../../com.aspose.cells/pagesetup\#getOrientation--) |
| [setPaperSize(int value)](#setPaperSize-int-) | Please see the getter of this property: [getPaperSize()](../../com.aspose.cells/pagesetup\#getPaperSize--) |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Please see the getter of this property: [isPercentScale()](../../com.aspose.cells/pagesetup\#isPercentScale--) |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Sets an image in the header/footer of a worksheet. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Please see the getter of this property: [getPrintArea()](../../com.aspose.cells/pagesetup\#getPrintArea--) |
| [setPrintComments(int value)](#setPrintComments-int-) | Please see the getter of this property: [getPrintComments()](../../com.aspose.cells/pagesetup\#getPrintComments--) |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Please see the getter of this property: [getPrintCopies()](../../com.aspose.cells/pagesetup\#getPrintCopies--) |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Please see the getter of this property: [getPrintDraft()](../../com.aspose.cells/pagesetup\#getPrintDraft--) |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Please see the getter of this property: [getPrintErrors()](../../com.aspose.cells/pagesetup\#getPrintErrors--) |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Please see the getter of this property: [getPrintGridlines()](../../com.aspose.cells/pagesetup\#getPrintGridlines--) |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Please see the getter of this property: [getPrintHeadings()](../../com.aspose.cells/pagesetup\#getPrintHeadings--) |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Please see the getter of this property: [getPrintQuality()](../../com.aspose.cells/pagesetup\#getPrintQuality--) |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Please see the getter of this property: [getPrintTitleColumns()](../../com.aspose.cells/pagesetup\#getPrintTitleColumns--) |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Please see the getter of this property: [getPrintTitleRows()](../../com.aspose.cells/pagesetup\#getPrintTitleRows--) |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Please see the getter of this property: [getPrinterSettings()](../../com.aspose.cells/pagesetup\#getPrinterSettings--) |
| [setRightMargin(double value)](#setRightMargin-double-) | Please see the getter of this property: [getRightMargin()](../../com.aspose.cells/pagesetup\#getRightMargin--) |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Please see the getter of this property: [getRightMarginInch()](../../com.aspose.cells/pagesetup\#getRightMarginInch--) |
| [setTopMargin(double value)](#setTopMargin-double-) | Please see the getter of this property: [getTopMargin()](../../com.aspose.cells/pagesetup\#getTopMargin--) |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Please see the getter of this property: [getTopMarginInch()](../../com.aspose.cells/pagesetup\#getTopMarginInch--) |
| [setZoom(int value)](#setZoom-int-) | Please see the getter of this property: [getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Clears header and footer setting.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Copies the setting of the page setup.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | The source. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | The copy options. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Sets the custom paper size, in unit of inches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| width | double | The width of the paper. |
| height | double | The height of the paper. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Represents if elements of the document will be printed in black and white.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Represents the size of the bottom margin, in unit of centimeters.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Represents the size of the bottom margin, in unit of inches.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Represent if the sheet is printed centered horizontally.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Represent if the sheet is printed centered vertically.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


Gets all commands of header or footer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| headerFooterScript | java.lang.String | The header/footer script |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Returns all commands of header or footer.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Gets a script formatting the even footer of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Gets a script formatting the even header of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Gets a script formatting the first page footer of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Gets a script formatting the first page header of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Represents the first page number that will be used when this sheet is printed.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesWide as zero if you want to fit all rows on one page.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesTall as zero if you want to fit all columns on one page.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Gets a script formatting the footer of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Represents the distance from the bottom of the page to the footer, in unit of centimeters.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Represents the distance from the bottom of the page to the footer, in unit of inches.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Gets a script formatting the header of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Represents the distance from the top of the page to the header, in unit of centimeters.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Represents the distance from the top of the page to the header, in unit of inches.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Represents the size of the left margin, in unit of centimeters.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Represents the size of the left margin, in unit of inches.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Gets the background of ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Represents page print orientation.

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Gets the height of the paper in unit of inches , considered page orientation.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Represents the size of the paper.

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Gets the width of the paper in unit of inches, considered page orientation.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Gets the [Picture](../../com.aspose.cells/picture) object of the header / footer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether getting the picture of first page header/footer. |
| isEven | boolean | Indicates whether getting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether getting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Gets the [Picture](../../com.aspose.cells/picture) object of the header / footer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | boolean | Indicates whether it is in the header or footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Represents the range to be printed.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Represents the way comments are printed with the sheet.

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Get and sets number of copies to print.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Represents if the sheet will be printed without graphics.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Specifies the type of print error displayed.

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Represents if cell gridlines are printed on the page.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Represents if row and column headings are printed with this page.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Represents the print quality.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Represents the columns that contain the cells to be repeated on the left side of each page.

```
pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


Represents the rows that contain the cells to be repeated at the top of each page.

```
pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


Gets and sets the settings of the default printer.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Represents the size of the right margin, in unit of centimeters.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Represents the size of the right margin, in unit of inches.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Represents the size of the top margin, in unit of centimeters.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Represents the size of the top margin, in unit of inches.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Represents the scaling factor in percent. It should be between 10 and 400.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


Indicates whether the first the page number is automatically assigned.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Indicates whether the paper size is automatic.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


True means that the header/footer of the first page is different with other pages.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


True means that the header/footer of the odd pages is different with odd pages.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


Please see the getter of this property: [isAutoFirstPageNumber()](../../com.aspose.cells/pagesetup\#isAutoFirstPageNumber--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Please see the getter of this property: [getBlackAndWhite()](../../com.aspose.cells/pagesetup\#getBlackAndWhite--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Please see the getter of this property: [getBottomMargin()](../../com.aspose.cells/pagesetup\#getBottomMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Please see the getter of this property: [getBottomMarginInch()](../../com.aspose.cells/pagesetup\#getBottomMarginInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Please see the getter of this property: [getCenterHorizontally()](../../com.aspose.cells/pagesetup\#getCenterHorizontally--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Please see the getter of this property: [getCenterVertically()](../../com.aspose.cells/pagesetup\#getCenterVertically--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | java.lang.String | Footer format script. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | java.lang.String | Header format script. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Sets a script formatting the first page footer of an Excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | java.lang.String | Footer format script. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | java.lang.String | Header format script. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Please see the getter of this property: [getFirstPageNumber()](../../com.aspose.cells/pagesetup\#getFirstPageNumber--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Sets the number of pages the worksheet will be scaled to when it's printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wide | int | Pages wide. |
| tall | int | Pages tall. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Please see the getter of this property: [getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Please see the getter of this property: [getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Sets a script formatting the footer of an Excel file.

Script commands:

    | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
    | Command                    | Description                                                                                                                                             |
    | &P                         | Current page number\\u9286\\u20ac                                                                                                                       |
    | &N                         | Page count\\u9286\\u20ac                                                                                                                                |
    | &D                         | Current date\\u9286\\u20ac                                                                                                                              |
    | &T                         | Current time                                                                                                                                            |
    | &A                         | Sheet name                                                                                                                                              |
    | &F                         | File name without path                                                                                                                                  |
    | &"<FontName>"              | Font name, for example: &"Arial"                                                                                                                        |
    | &"<FontName>, <FontStyle>" | Font name and font style, for example: &"Arial,Bold"                                                                                                    |
    | &<FontSize>                | Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. |
    | &K<RRGGBB>                 | Font color, for example(RED): &KFF0000                                                                                                                  |
    | &G                         | Image script                                                                                                                                            |

    |

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | java.lang.String | Footer format script. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Please see the getter of this property: [getFooterMargin()](../../com.aspose.cells/pagesetup\#getFooterMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Please see the getter of this property: [getFooterMarginInch()](../../com.aspose.cells/pagesetup\#getFooterMarginInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Sets an image in the footer of a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerPicture | byte[] | Image data. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Please see the getter of this property: [isHFAlignMargins()](../../com.aspose.cells/pagesetup\#isHFAlignMargins--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


Please see the getter of this property: [isHFDiffFirst()](../../com.aspose.cells/pagesetup\#isHFDiffFirst--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


Please see the getter of this property: [isHFDiffOddEven()](../../com.aspose.cells/pagesetup\#isHFDiffOddEven--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Please see the getter of this property: [isHFScaleWithDoc()](../../com.aspose.cells/pagesetup\#isHFScaleWithDoc--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Sets a script formatting the header of an Excel file.

Script commands:

    | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
    | Command                    | Description                                                                                                                                             |
    | &P                         | Current page number\\u9286\\u20ac                                                                                                                       |
    | &N                         | Page count\\u9286\\u20ac                                                                                                                                |
    | &D                         | Current date\\u9286\\u20ac                                                                                                                              |
    | &T                         | Current time                                                                                                                                            |
    | &A                         | Sheet name                                                                                                                                              |
    | &F                         | File name without path                                                                                                                                  |
    | &"<FontName>"              | Font name, for example: &"Arial"                                                                                                                        |
    | &"<FontName>, <FontStyle>" | Font name and font style, for example: &"Arial,Bold"                                                                                                    |
    | &<FontSize>                | Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. |
    | &K<RRGGBB>                 | Font color, for example(RED): &KFF0000                                                                                                                  |
    | &G                         | Image script                                                                                                                                            |

    |

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | java.lang.String | Header format script. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Please see the getter of this property: [getHeaderMargin()](../../com.aspose.cells/pagesetup\#getHeaderMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Please see the getter of this property: [getHeaderMarginInch()](../../com.aspose.cells/pagesetup\#getHeaderMarginInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Sets an image in the header of a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerPicture | byte[] | Image data. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Please see the getter of this property: [getLeftMargin()](../../com.aspose.cells/pagesetup\#getLeftMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Please see the getter of this property: [getLeftMarginInch()](../../com.aspose.cells/pagesetup\#getLeftMarginInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Please see the getter of this property: [getOrder()](../../com.aspose.cells/pagesetup\#getOrder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Please see the getter of this property: [getOrientation()](../../com.aspose.cells/pagesetup\#getOrientation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Please see the getter of this property: [getPaperSize()](../../com.aspose.cells/pagesetup\#getPaperSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Please see the getter of this property: [isPercentScale()](../../com.aspose.cells/pagesetup\#isPercentScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Sets an image in the header/footer of a worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether setting the picture of first page header/footer. |
| isEven | boolean | Indicates whether setting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether setting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| imageData | byte[] | Image data. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Please see the getter of this property: [getPrintArea()](../../com.aspose.cells/pagesetup\#getPrintArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Please see the getter of this property: [getPrintComments()](../../com.aspose.cells/pagesetup\#getPrintComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Please see the getter of this property: [getPrintCopies()](../../com.aspose.cells/pagesetup\#getPrintCopies--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Please see the getter of this property: [getPrintDraft()](../../com.aspose.cells/pagesetup\#getPrintDraft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Please see the getter of this property: [getPrintErrors()](../../com.aspose.cells/pagesetup\#getPrintErrors--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Please see the getter of this property: [getPrintGridlines()](../../com.aspose.cells/pagesetup\#getPrintGridlines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Please see the getter of this property: [getPrintHeadings()](../../com.aspose.cells/pagesetup\#getPrintHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Please see the getter of this property: [getPrintQuality()](../../com.aspose.cells/pagesetup\#getPrintQuality--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Please see the getter of this property: [getPrintTitleColumns()](../../com.aspose.cells/pagesetup\#getPrintTitleColumns--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Please see the getter of this property: [getPrintTitleRows()](../../com.aspose.cells/pagesetup\#getPrintTitleRows--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Please see the getter of this property: [getPrinterSettings()](../../com.aspose.cells/pagesetup\#getPrinterSettings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Please see the getter of this property: [getRightMargin()](../../com.aspose.cells/pagesetup\#getRightMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Please see the getter of this property: [getRightMarginInch()](../../com.aspose.cells/pagesetup\#getRightMarginInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Please see the getter of this property: [getTopMargin()](../../com.aspose.cells/pagesetup\#getTopMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Please see the getter of this property: [getTopMarginInch()](../../com.aspose.cells/pagesetup\#getTopMarginInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Please see the getter of this property: [getZoom()](../../com.aspose.cells/pagesetup\#getZoom--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

