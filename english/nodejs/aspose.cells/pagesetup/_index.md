---
title: "PageSetup"
linktitle: "PageSetup"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents the page setup description."
type: docs
weight: 2510
url: /nodejs/aspose.cells/pagesetup/
---

## PageSetup class

Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.

## Methods

| Name | Description |
| --- | --- |
| [clearHeaderFooter()](#clearheaderfooter) | Clears header and footer setting. |
| [copy(source, copyOptions)](#copy) | Copies the setting of the page setup. |
| [customPaperSize(width, height)](#custompapersize) | Sets the custom paper size, in unit of inches. |
| [getBlackAndWhite()](#getblackandwhite) | Represents if elements of the document will be printed in black and white. |
| [getBottomMargin()](#getbottommargin) | Represents the size of the bottom margin, in unit of centimeters. |
| [getBottomMarginInch()](#getbottommargininch) | Represents the size of the bottom margin, in unit of inches. |
| [getCenterHorizontally()](#getcenterhorizontally) | Represent if the sheet is printed centered horizontally. |
| [getCenterVertically()](#getcentervertically) | Represent if the sheet is printed centered vertically. |
| [getCommands(headerFooterScript)](#getcommands) | Gets all commands of header or footer. |
| [getEvenFooter(section)](#getevenfooter) | Gets a script formatting the even footer of an Excel file. |
| [getEvenHeader(section)](#getevenheader) | Gets a script formatting the even header of an Excel file. |
| [getFirstPageFooter(section)](#getfirstpagefooter) | Gets a script formatting the first page footer of an Excel file. |
| [getFirstPageHeader(section)](#getfirstpageheader) | Gets a script formatting the first page header of an Excel file. |
| [getFirstPageNumber()](#getfirstpagenumber) | Represents the first page number that will be used when this sheet is printed. |
| [getFitToPagesTall()](#getfittopagestall) | Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have  |
| [getFitToPagesWide()](#getfittopageswide) | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have  |
| [getFooter(section)](#getfooter) | Gets a script formatting the footer of an Excel file. |
| [getFooterMargin()](#getfootermargin) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [getFooterMarginInch()](#getfootermargininch) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [getHeader(section)](#getheader) | Gets a script formatting the header of an Excel file. |
| [getHeaderMargin()](#getheadermargin) | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [getHeaderMarginInch()](#getheadermargininch) | Represents the distance from the top of the page to the header, in unit of inches. |
| [getLeftMargin()](#getleftmargin) | Represents the size of the left margin, in unit of centimeters. |
| [getLeftMarginInch()](#getleftmargininch) | Represents the size of the left margin, in unit of inches. |
| [getODSPageBackground()](#getodspagebackground) | Gets the background of ODS. |
| [getOrder()](#getorder) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. The value of the propert |
| [getOrientation()](#getorientation) | Represents page print orientation. The value of the property is PageOrientationType integer constant. |
| [getPaperHeight()](#getpaperheight) | Gets the height of the paper in unit of inches , considered page orientation. |
| [getPaperSize()](#getpapersize) | Represents the size of the paper. The value of the property is PaperSizeType integer constant. |
| [getPaperWidth()](#getpaperwidth) | Gets the width of the paper in unit of inches, considered page orientation. |
| [getPicture(isHeader, section)](#getpicture) | Gets the Picture object of the header / footer. |
| [getPicture(isFirst, isEven, isHeader, section)](#getpicture-1) | Gets the Picture object of the header / footer. |
| [getPrintArea()](#getprintarea) | Represents the range to be printed. |
| [getPrintComments()](#getprintcomments) | Represents the way comments are printed with the sheet. The value of the property is PrintCommentsType integer constant. |
| [getPrintCopies()](#getprintcopies) | Get and sets number of copies to print. |
| [getPrintDraft()](#getprintdraft) | Represents if the sheet will be printed without graphics. |
| [getPrintErrors()](#getprinterrors) | Specifies the type of print error displayed. The value of the property is PrintErrorsType integer constant. |
| [getPrintGridlines()](#getprintgridlines) | Represents if cell gridlines are printed on the page. |
| [getPrintHeadings()](#getprintheadings) | Represents if row and column headings are printed with this page. |
| [getPrintQuality()](#getprintquality) | Represents the print quality. |
| [getPrintTitleColumns()](#getprinttitlecolumns) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [getPrintTitleRows()](#getprinttitlerows) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [getPrinterSettings()](#getprintersettings) | Gets and sets the settings of the default printer. |
| [getRightMargin()](#getrightmargin) | Represents the size of the right margin, in unit of centimeters. |
| [getRightMarginInch()](#getrightmargininch) | Represents the size of the right margin, in unit of inches. |
| [getTopMargin()](#gettopmargin) | Represents the size of the top margin, in unit of centimeters. |
| [getTopMarginInch()](#gettopmargininch) | Represents the size of the top margin, in unit of inches. |
| [getZoom()](#getzoom) | Represents the scaling factor in percent. It should be between 10 and 400. |
| [isAutoFirstPageNumber()](#isautofirstpagenumber) | Indicates whether the first the page number is automatically assigned. |
| [isAutomaticPaperSize()](#isautomaticpapersize) | Indicates whether the paper size is automatic. |
| [isHFAlignMargins()](#ishfalignmargins) | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header |
| [isHFDiffFirst()](#ishfdifffirst) | True means that the header/footer of the first page is different with other pages. |
| [isHFDiffOddEven()](#ishfdiffoddeven) | True means that the header/footer of the odd pages is different with odd pages. |
| [isHFScaleWithDoc()](#ishfscalewithdoc) | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [isPercentScale()](#ispercentscale) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [setAutoFirstPageNumber()](#setautofirstpagenumber) | Indicates whether the first the page number is automatically assigned. |
| [setBlackAndWhite()](#setblackandwhite) | Represents if elements of the document will be printed in black and white. |
| [setBottomMargin()](#setbottommargin) | Represents the size of the bottom margin, in unit of centimeters. |
| [setBottomMarginInch()](#setbottommargininch) | Represents the size of the bottom margin, in unit of inches. |
| [setCenterHorizontally()](#setcenterhorizontally) | Represent if the sheet is printed centered horizontally. |
| [setCenterVertically()](#setcentervertically) | Represent if the sheet is printed centered vertically. |
| [setEvenFooter(section, footerScript)](#setevenfooter) | Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [setEvenHeader(section, headerScript)](#setevenheader) | Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [setFirstPageFooter(section, footerScript)](#setfirstpagefooter) | Sets a script formatting the first page footer of an Excel file. |
| [setFirstPageHeader(section, headerScript)](#setfirstpageheader) | Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true. |
| [setFirstPageNumber()](#setfirstpagenumber) | Represents the first page number that will be used when this sheet is printed. |
| [setFitToPages(wide, tall)](#setfittopages) | Sets the number of pages the worksheet will be scaled to when it's printed. |
| [setFitToPagesTall()](#setfittopagestall) | Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have  |
| [setFitToPagesWide()](#setfittopageswide) | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have  |
| [setFooter(section, footerScript)](#setfooter) | Sets a script formatting the footer of an Excel file. Script commands:CommandDescription&PCurrent page number &NPage cou |
| [setFooterMargin()](#setfootermargin) | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [setFooterMarginInch()](#setfootermargininch) | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [setFooterPicture(section, footerPicture)](#setfooterpicture) | Sets an image in the footer of a worksheet. |
| [setHFAlignMargins()](#sethfalignmargins) | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header |
| [setHFDiffFirst()](#sethfdifffirst) | True means that the header/footer of the first page is different with other pages. |
| [setHFDiffOddEven()](#sethfdiffoddeven) | True means that the header/footer of the odd pages is different with odd pages. |
| [setHFScaleWithDoc()](#sethfscalewithdoc) | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [setHeader(section, headerScript)](#setheader) | Sets a script formatting the header of an Excel file. Script commands:CommandDescription&PCurrent page number &NPage cou |
| [setHeaderMargin()](#setheadermargin) | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [setHeaderMarginInch()](#setheadermargininch) | Represents the distance from the top of the page to the header, in unit of inches. |
| [setHeaderPicture(section, headerPicture)](#setheaderpicture) | Sets an image in the header of a worksheet. |
| [setLeftMargin()](#setleftmargin) | Represents the size of the left margin, in unit of centimeters. |
| [setLeftMarginInch()](#setleftmargininch) | Represents the size of the left margin, in unit of inches. |
| [setOrder()](#setorder) | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. The value of the propert |
| [setOrientation()](#setorientation) | Represents page print orientation. The value of the property is PageOrientationType integer constant. |
| [setPaperSize()](#setpapersize) | Represents the size of the paper. The value of the property is PaperSizeType integer constant. |
| [setPercentScale()](#setpercentscale) | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [setPicture(isFirst, isEven, isHeader, section, imageData)](#setpicture) | Sets an image in the header/footer of a worksheet. |
| [setPrintArea()](#setprintarea) | Represents the range to be printed. |
| [setPrintComments()](#setprintcomments) | Represents the way comments are printed with the sheet. The value of the property is PrintCommentsType integer constant. |
| [setPrintCopies()](#setprintcopies) | Get and sets number of copies to print. |
| [setPrintDraft()](#setprintdraft) | Represents if the sheet will be printed without graphics. |
| [setPrintErrors()](#setprinterrors) | Specifies the type of print error displayed. The value of the property is PrintErrorsType integer constant. |
| [setPrintGridlines()](#setprintgridlines) | Represents if cell gridlines are printed on the page. |
| [setPrintHeadings()](#setprintheadings) | Represents if row and column headings are printed with this page. |
| [setPrintQuality()](#setprintquality) | Represents the print quality. |
| [setPrintTitleColumns()](#setprinttitlecolumns) | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [setPrintTitleRows()](#setprinttitlerows) | Represents the rows that contain the cells to be repeated at the top of each page. |
| [setPrinterSettings()](#setprintersettings) | Gets and sets the settings of the default printer. |
| [setRightMargin()](#setrightmargin) | Represents the size of the right margin, in unit of centimeters. |
| [setRightMarginInch()](#setrightmargininch) | Represents the size of the right margin, in unit of inches. |
| [setTopMargin()](#settopmargin) | Represents the size of the top margin, in unit of centimeters. |
| [setTopMarginInch()](#settopmargininch) | Represents the size of the top margin, in unit of inches. |
| [setZoom()](#setzoom) | Represents the scaling factor in percent. It should be between 10 and 400. |

### clearHeaderFooter() {#clearheaderfooter}

Clears header and footer setting.

### copy(source, copyOptions) {#copy}

Copies the setting of the page setup.

| Parameter | Type | Description |
| --- | --- | --- |
| source | PageSetup | The source. |
| copyOptions | CopyOptions | The copy options. |

### customPaperSize(width, height) {#custompapersize}

Sets the custom paper size, in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| width | Number | The width of the paper. |
| height | Number | The height of the paper. |

### getBlackAndWhite() {#getblackandwhite}

Represents if elements of the document will be printed in black and white.

### getBottomMargin() {#getbottommargin}

Represents the size of the bottom margin, in unit of centimeters.

### getBottomMarginInch() {#getbottommargininch}

Represents the size of the bottom margin, in unit of inches.

### getCenterHorizontally() {#getcenterhorizontally}

Represent if the sheet is printed centered horizontally.

### getCenterVertically() {#getcentervertically}

Represent if the sheet is printed centered vertically.

### getCommands(headerFooterScript) {#getcommands}

Gets all commands of header or footer.

| Parameter | Type | Description |
| --- | --- | --- |
| headerFooterScript | String | The header/footer script |

**Returns:** Array ofHeaderFooterCommand — `Array ofHeaderFooterCommand` Returns all commands of header or footer.

### getEvenFooter(section) {#getevenfooter}

Gets a script formatting the even footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

### getEvenHeader(section) {#getevenheader}

Gets a script formatting the even header of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

### getFirstPageFooter(section) {#getfirstpagefooter}

Gets a script formatting the first page footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

### getFirstPageHeader(section) {#getfirstpageheader}

Gets a script formatting the first page header of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

### getFirstPageNumber() {#getfirstpagenumber}

Represents the first page number that will be used when this sheet is printed.

### getFitToPagesTall() {#getfittopagestall}

Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesWide as zero if you want to fit all rows on one page.

### getFitToPagesWide() {#getfittopageswide}

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesTall as zero if you want to fit all columns on one page.

### getFooter(section) {#getfooter}

Gets a script formatting the footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

### getFooterMargin() {#getfootermargin}

Represents the distance from the bottom of the page to the footer, in unit of centimeters.

### getFooterMarginInch() {#getfootermargininch}

Represents the distance from the bottom of the page to the footer, in unit of inches.

### getHeader(section) {#getheader}

Gets a script formatting the header of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

### getHeaderMargin() {#getheadermargin}

Represents the distance from the top of the page to the header, in unit of centimeters.

### getHeaderMarginInch() {#getheadermargininch}

Represents the distance from the top of the page to the header, in unit of inches.

### getLeftMargin() {#getleftmargin}

Represents the size of the left margin, in unit of centimeters.

### getLeftMarginInch() {#getleftmargininch}

Represents the size of the left margin, in unit of inches.

### getODSPageBackground() {#getodspagebackground}

Gets the background of ODS.

### getOrder() {#getorder}

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. The value of the property is PrintOrderType integer constant.

### getOrientation() {#getorientation}

Represents page print orientation. The value of the property is PageOrientationType integer constant.

### getPaperHeight() {#getpaperheight}

Gets the height of the paper in unit of inches , considered page orientation.

### getPaperSize() {#getpapersize}

Represents the size of the paper. The value of the property is PaperSizeType integer constant.

### getPaperWidth() {#getpaperwidth}

Gets the width of the paper in unit of inches, considered page orientation.

### getPicture(isHeader, section) {#getpicture}

Gets the Picture object of the header / footer.

| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | boolean | Indicates whether it is in the header or footer. |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:** Picture — `Picture` Returns Picture object. Returns null if there is no picture.

### getPicture(isFirst, isEven, isHeader, section) {#getpicture-1}

Gets the Picture object of the header / footer.

| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether getting the picture of first page header/footer. |
| isEven | boolean | Indicates whether getting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether getting the picture of header/footer. |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:** Picture — `Picture` Returns Picture object.

### getPrintArea() {#getprintarea}

Represents the range to be printed.

### getPrintComments() {#getprintcomments}

Represents the way comments are printed with the sheet. The value of the property is PrintCommentsType integer constant.

### getPrintCopies() {#getprintcopies}

Get and sets number of copies to print.

### getPrintDraft() {#getprintdraft}

Represents if the sheet will be printed without graphics.

### getPrintErrors() {#getprinterrors}

Specifies the type of print error displayed. The value of the property is PrintErrorsType integer constant.

### getPrintGridlines() {#getprintgridlines}

Represents if cell gridlines are printed on the page.

### getPrintHeadings() {#getprintheadings}

Represents if row and column headings are printed with this page.

### getPrintQuality() {#getprintquality}

Represents the print quality.

### getPrintTitleColumns() {#getprinttitlecolumns}

Represents the columns that contain the cells to be repeated on the left side of each page.

### getPrintTitleRows() {#getprinttitlerows}

Represents the rows that contain the cells to be repeated at the top of each page.

### getPrinterSettings() {#getprintersettings}

Gets and sets the settings of the default printer.

### getRightMargin() {#getrightmargin}

Represents the size of the right margin, in unit of centimeters.

### getRightMarginInch() {#getrightmargininch}

Represents the size of the right margin, in unit of inches.

### getTopMargin() {#gettopmargin}

Represents the size of the top margin, in unit of centimeters.

### getTopMarginInch() {#gettopmargininch}

Represents the size of the top margin, in unit of inches.

### getZoom() {#getzoom}

Represents the scaling factor in percent. It should be between 10 and 400.

### isAutoFirstPageNumber() {#isautofirstpagenumber}

Indicates whether the first the page number is automatically assigned.

### isAutomaticPaperSize() {#isautomaticpapersize}

Indicates whether the paper size is automatic.

### isHFAlignMargins() {#ishfalignmargins}

Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

### isHFDiffFirst() {#ishfdifffirst}

True means that the header/footer of the first page is different with other pages.

### isHFDiffOddEven() {#ishfdiffoddeven}

True means that the header/footer of the odd pages is different with odd pages.

### isHFScaleWithDoc() {#ishfscalewithdoc}

Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

### isPercentScale() {#ispercentscale}

If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

### setAutoFirstPageNumber() {#setautofirstpagenumber}

Indicates whether the first the page number is automatically assigned.

### setBlackAndWhite() {#setblackandwhite}

Represents if elements of the document will be printed in black and white.

### setBottomMargin() {#setbottommargin}

Represents the size of the bottom margin, in unit of centimeters.

### setBottomMarginInch() {#setbottommargininch}

Represents the size of the bottom margin, in unit of inches.

### setCenterHorizontally() {#setcenterhorizontally}

Represent if the sheet is printed centered horizontally.

### setCenterVertically() {#setcentervertically}

Represent if the sheet is printed centered vertically.

### setEvenFooter(section, footerScript) {#setevenfooter}

Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### setEvenHeader(section, headerScript) {#setevenheader}

Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### setFirstPageFooter(section, footerScript) {#setfirstpagefooter}

Sets a script formatting the first page footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### setFirstPageHeader(section, headerScript) {#setfirstpageheader}

Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### setFirstPageNumber() {#setfirstpagenumber}

Represents the first page number that will be used when this sheet is printed.

### setFitToPages(wide, tall) {#setfittopages}

Sets the number of pages the worksheet will be scaled to when it's printed.

| Parameter | Type | Description |
| --- | --- | --- |
| wide | Number | Pages wide. |
| tall | Number | Pages tall. |

### setFitToPagesTall() {#setfittopagestall}

Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesWide as zero if you want to fit all rows on one page.

### setFitToPagesWide() {#setfittopageswide}

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesTall as zero if you want to fit all columns on one page.

### setFooter(section, footerScript) {#setfooter}

Sets a script formatting the footer of an Excel file. Script commands:CommandDescription&PCurrent page number &NPage count &DCurrent date &TCurrent time&ASheet name&FFile name without path&" "Font name, for example: &"Arial"&" , "Font name and font style, for example: &"Arial,Bold"& Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.&K Font color, for example(RED): &KFF0000&GImage script For example: "&Arial,Bold&8Footer Note"

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### setFooterMargin() {#setfootermargin}

Represents the distance from the bottom of the page to the footer, in unit of centimeters.

### setFooterMarginInch() {#setfootermargininch}

Represents the distance from the bottom of the page to the footer, in unit of inches.

### setFooterPicture(section, footerPicture) {#setfooterpicture}

Sets an image in the footer of a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerPicture | Array of byte | Image data. |

**Returns:** Picture — `Picture` Returns Picture object.

### setHFAlignMargins() {#sethfalignmargins}

Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

### setHFDiffFirst() {#sethfdifffirst}

True means that the header/footer of the first page is different with other pages.

### setHFDiffOddEven() {#sethfdiffoddeven}

True means that the header/footer of the odd pages is different with odd pages.

### setHFScaleWithDoc() {#sethfscalewithdoc}

Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

### setHeader(section, headerScript) {#setheader}

Sets a script formatting the header of an Excel file. Script commands:CommandDescription&PCurrent page number &NPage count &DCurrent date &TCurrent time&ASheet name&FFile name without path&" "Font name, for example: &"Arial"&" , "Font name and font style, for example: &"Arial,Bold"& Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.&K Font color, for example(RED): &KFF0000&GImage script For example: "&Arial,Bold&8Header Note"

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### setHeaderMargin() {#setheadermargin}

Represents the distance from the top of the page to the header, in unit of centimeters.

### setHeaderMarginInch() {#setheadermargininch}

Represents the distance from the top of the page to the header, in unit of inches.

### setHeaderPicture(section, headerPicture) {#setheaderpicture}

Sets an image in the header of a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerPicture | Array of byte | Image data. |

**Returns:** Picture — `Picture` Returns Picture object.

### setLeftMargin() {#setleftmargin}

Represents the size of the left margin, in unit of centimeters.

### setLeftMarginInch() {#setleftmargininch}

Represents the size of the left margin, in unit of inches.

### setOrder() {#setorder}

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. The value of the property is PrintOrderType integer constant.

### setOrientation() {#setorientation}

Represents page print orientation. The value of the property is PageOrientationType integer constant.

### setPaperSize() {#setpapersize}

Represents the size of the paper. The value of the property is PaperSizeType integer constant.

### setPercentScale() {#setpercentscale}

If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

### setPicture(isFirst, isEven, isHeader, section, imageData) {#setpicture}

Sets an image in the header/footer of a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether setting the picture of first page header/footer. |
| isEven | boolean | Indicates whether setting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether setting the picture of header/footer. |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| imageData | Array of byte | Image data. |

**Returns:** Picture — `Picture` Returns Picture object.

### setPrintArea() {#setprintarea}

Represents the range to be printed.

### setPrintComments() {#setprintcomments}

Represents the way comments are printed with the sheet. The value of the property is PrintCommentsType integer constant.

### setPrintCopies() {#setprintcopies}

Get and sets number of copies to print.

### setPrintDraft() {#setprintdraft}

Represents if the sheet will be printed without graphics.

### setPrintErrors() {#setprinterrors}

Specifies the type of print error displayed. The value of the property is PrintErrorsType integer constant.

### setPrintGridlines() {#setprintgridlines}

Represents if cell gridlines are printed on the page.

### setPrintHeadings() {#setprintheadings}

Represents if row and column headings are printed with this page.

### setPrintQuality() {#setprintquality}

Represents the print quality.

### setPrintTitleColumns() {#setprinttitlecolumns}

Represents the columns that contain the cells to be repeated on the left side of each page.

### setPrintTitleRows() {#setprinttitlerows}

Represents the rows that contain the cells to be repeated at the top of each page.

### setPrinterSettings() {#setprintersettings}

Gets and sets the settings of the default printer.

### setRightMargin() {#setrightmargin}

Represents the size of the right margin, in unit of centimeters.

### setRightMarginInch() {#setrightmargininch}

Represents the size of the right margin, in unit of inches.

### setTopMargin() {#settopmargin}

Represents the size of the top margin, in unit of centimeters.

### setTopMarginInch() {#settopmargininch}

Represents the size of the top margin, in unit of inches.

### setZoom() {#setzoom}

Represents the scaling factor in percent. It should be between 10 and 400.
