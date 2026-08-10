---
title: "PageSetup Class"
linktitle: "PageSetup"
articleTitle: "PageSetup"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents the page setup description."
type: docs
weight: 4180
url: /python-java/asposecells.api/pagesetup/
---

## PageSetup class

Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ODSPageBackground](#odspagebackground) | OdsPageBackground | Gets the background of ODS. |
| [PrintArea](#printarea) | String | Represents the range to be printed. |
| [PrintTitleColumns](#printtitlecolumns) | String | Represents the columns that contain the cells to be repeated on the left side of each page. |
| [PrintTitleRows](#printtitlerows) | String | Represents the rows that contain the cells to be repeated at the top of each page. |
| [BlackAndWhite](#blackandwhite) | boolean | Represents if elements of the document will be printed in black and white. |
| [CenterHorizontally](#centerhorizontally) | boolean | Represent if the sheet is printed centered horizontally. |
| [CenterVertically](#centervertically) | boolean | Represent if the sheet is printed centered vertically. |
| [PrintDraft](#printdraft) | boolean | Represents if the sheet will be printed without graphics. |
| [FooterMargin](#footermargin) | float | Represents the distance from the bottom of the page to the footer, in unit of centimeters. |
| [FooterMarginInch](#footermargininch) | float | Represents the distance from the bottom of the page to the footer, in unit of inches. |
| [HeaderMargin](#headermargin) | float | Represents the distance from the top of the page to the header, in unit of centimeters. |
| [HeaderMarginInch](#headermargininch) | float | Represents the distance from the top of the page to the header, in unit of inches. |
| [PrinterSettings](#printersettings) | byte[] | Gets and sets the settings of the default printer. |
| [LeftMargin](#leftmargin) | float | Represents the size of the left margin, in unit of centimeters. |
| [LeftMarginInch](#leftmargininch) | float | Represents the size of the left margin, in unit of inches. |
| [RightMargin](#rightmargin) | float | Represents the size of the right margin, in unit of centimeters. |
| [RightMarginInch](#rightmargininch) | float | Represents the size of the right margin, in unit of inches. |
| [TopMargin](#topmargin) | float | Represents the size of the top margin, in unit of centimeters. |
| [TopMarginInch](#topmargininch) | float | Represents the size of the top margin, in unit of inches. |
| [BottomMargin](#bottommargin) | float | Represents the size of the bottom margin, in unit of centimeters. |
| [BottomMarginInch](#bottommargininch) | float | Represents the size of the bottom margin, in unit of inches. |
| [FirstPageNumber](#firstpagenumber) | int | Represents the first page number that will be used when this sheet is printed. |
| [FitToPagesTall](#fittopagestall) | int | Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have  |
| [FitToPagesWide](#fittopageswide) | int | Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have  |
| [IsPercentScale](#ispercentscale) | boolean | If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled. |
| [Order](#order) | int | Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. The value of the propert |
| [IsAutomaticPaperSize](#isautomaticpapersize) | boolean | Indicates whether the paper size is automatic. |
| [PaperSize](#papersize) | int | Represents the size of the paper. The value of the property is PaperSizeType integer constant. |
| [PaperWidth](#paperwidth) | float | Gets the width of the paper in unit of inches, considered page orientation. |
| [PaperHeight](#paperheight) | float | Gets the height of the paper in unit of inches , considered page orientation. |
| [Orientation](#orientation) | int | Represents page print orientation. The value of the property is PageOrientationType integer constant. |
| [PrintComments](#printcomments) | int | Represents the way comments are printed with the sheet. The value of the property is PrintCommentsType integer constant. |
| [PrintErrors](#printerrors) | int | Specifies the type of print error displayed. The value of the property is PrintErrorsType integer constant. |
| [PrintHeadings](#printheadings) | boolean | Represents if row and column headings are printed with this page. |
| [PrintGridlines](#printgridlines) | boolean | Represents if cell gridlines are printed on the page. |
| [Zoom](#zoom) | int | Represents the scaling factor in percent. It should be between 10 and 400. |
| [IsAutoFirstPageNumber](#isautofirstpagenumber) | boolean | Indicates whether the first the page number is automatically assigned. |
| [PrintQuality](#printquality) | int | Represents the print quality. |
| [PrintCopies](#printcopies) | int | Get and sets number of copies to print. |
| [IsHFDiffOddEven](#ishfdiffoddeven) | boolean | True means that the header/footer of the odd pages is different with odd pages. |
| [IsHFDiffFirst](#ishfdifffirst) | boolean | True means that the header/footer of the first page is different with other pages. |
| [IsHFScaleWithDoc](#ishfscalewithdoc) | boolean | Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007. |
| [IsHFAlignMargins](#ishfalignmargins) | boolean | Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header |

## Methods

| Name | Description |
| --- | --- |
| [setHeaderPicture](#setheaderpicture) | Sets an image in the header of a worksheet. |
| [setFooterPicture](#setfooterpicture) | Sets an image in the footer of a worksheet. |
| [setPicture](#setpicture) | Sets an image in the header/footer of a worksheet. |
| [getPicture](#getpicture) | Gets the Picture object of the header / footer. |
| [copy](#copy) | Copies the setting of the page setup. |
| [setFitToPages](#setfittopages) | Sets the number of pages the worksheet will be scaled to when it's printed. |
| [customPaperSize](#custompapersize) | Sets the custom paper size, in unit of inches. |
| [clearHeaderFooter](#clearheaderfooter) | Clears header and footer setting. |
| [getHeader](#getheader) | Gets a script formatting the header of an Excel file. |
| [getCommands](#getcommands) | Gets all commands of header or footer. |
| [getFooter](#getfooter) | Gets a script formatting the footer of an Excel file. |
| [setHeader](#setheader) | Sets a script formatting the header of an Excel file.

Script commands: Command Description &P Current page number &N Pa |
| [setFooter](#setfooter) | Sets a script formatting the footer of an Excel file.

Script commands: Command Description &P Current page number &N Pa |
| [setEvenHeader](#setevenheader) | Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [getEvenHeader](#getevenheader) | Gets a script formatting the even header of an Excel file. |
| [setEvenFooter](#setevenfooter) | Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true. |
| [getEvenFooter](#getevenfooter) | Gets a script formatting the even footer of an Excel file. |
| [setFirstPageHeader](#setfirstpageheader) | Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true. |
| [getFirstPageHeader](#getfirstpageheader) | Gets a script formatting the first page header of an Excel file. |
| [setFirstPageFooter](#setfirstpagefooter) | Sets a script formatting the first page footer of an Excel file. |
| [getFirstPageFooter](#getfirstpagefooter) | Gets a script formatting the first page footer of an Excel file. |

### PageSetup.ODSPageBackground property {#odspagebackground}

Gets the background of ODS.

**Type:** OdsPageBackground

### PageSetup.PrintArea property {#printarea}

Represents the range to be printed.

**Type:** String

### PageSetup.PrintTitleColumns property {#printtitlecolumns}

Represents the columns that contain the cells to be repeated on the left side of each page.

**Type:** String

### PageSetup.PrintTitleRows property {#printtitlerows}

Represents the rows that contain the cells to be repeated at the top of each page.

**Type:** String

### PageSetup.BlackAndWhite property {#blackandwhite}

Represents if elements of the document will be printed in black and white.

**Type:** boolean

### PageSetup.CenterHorizontally property {#centerhorizontally}

Represent if the sheet is printed centered horizontally.

**Type:** boolean

### PageSetup.CenterVertically property {#centervertically}

Represent if the sheet is printed centered vertically.

**Type:** boolean

### PageSetup.PrintDraft property {#printdraft}

Represents if the sheet will be printed without graphics.

**Type:** boolean

### PageSetup.FooterMargin property {#footermargin}

Represents the distance from the bottom of the page to the footer, in unit of centimeters.

**Type:** float

### PageSetup.FooterMarginInch property {#footermargininch}

Represents the distance from the bottom of the page to the footer, in unit of inches.

**Type:** float

### PageSetup.HeaderMargin property {#headermargin}

Represents the distance from the top of the page to the header, in unit of centimeters.

**Type:** float

### PageSetup.HeaderMarginInch property {#headermargininch}

Represents the distance from the top of the page to the header, in unit of inches.

**Type:** float

### PageSetup.PrinterSettings property {#printersettings}

Gets and sets the settings of the default printer.

**Type:** byte[]

### PageSetup.LeftMargin property {#leftmargin}

Represents the size of the left margin, in unit of centimeters.

**Type:** float

### PageSetup.LeftMarginInch property {#leftmargininch}

Represents the size of the left margin, in unit of inches.

**Type:** float

### PageSetup.RightMargin property {#rightmargin}

Represents the size of the right margin, in unit of centimeters.

**Type:** float

### PageSetup.RightMarginInch property {#rightmargininch}

Represents the size of the right margin, in unit of inches.

**Type:** float

### PageSetup.TopMargin property {#topmargin}

Represents the size of the top margin, in unit of centimeters.

**Type:** float

### PageSetup.TopMarginInch property {#topmargininch}

Represents the size of the top margin, in unit of inches.

**Type:** float

### PageSetup.BottomMargin property {#bottommargin}

Represents the size of the bottom margin, in unit of centimeters.

**Type:** float

### PageSetup.BottomMarginInch property {#bottommargininch}

Represents the size of the bottom margin, in unit of inches.

**Type:** float

### PageSetup.FirstPageNumber property {#firstpagenumber}

Represents the first page number that will be used when this sheet is printed.

**Type:** int

### PageSetup.FitToPagesTall property {#fittopagestall}

Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesWide as zero if you want to fit all rows on one page.

**Type:** int

### PageSetup.FitToPagesWide property {#fittopageswide}

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1. You have to set FitToPagesTall as zero if you want to fit all columns on one page.

**Type:** int

### PageSetup.IsPercentScale property {#ispercentscale}

If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

**Type:** boolean

### PageSetup.Order property {#order}

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet. The value of the property is PrintOrderType integer constant.

**Type:** int

### PageSetup.IsAutomaticPaperSize property {#isautomaticpapersize}

Indicates whether the paper size is automatic.

**Type:** boolean

### PageSetup.PaperSize property {#papersize}

Represents the size of the paper. The value of the property is PaperSizeType integer constant.

**Type:** int

### PageSetup.PaperWidth property {#paperwidth}

Gets the width of the paper in unit of inches, considered page orientation.

**Type:** float

### PageSetup.PaperHeight property {#paperheight}

Gets the height of the paper in unit of inches , considered page orientation.

**Type:** float

### PageSetup.Orientation property {#orientation}

Represents page print orientation. The value of the property is PageOrientationType integer constant.

**Type:** int

### PageSetup.PrintComments property {#printcomments}

Represents the way comments are printed with the sheet. The value of the property is PrintCommentsType integer constant.

**Type:** int

### PageSetup.PrintErrors property {#printerrors}

Specifies the type of print error displayed. The value of the property is PrintErrorsType integer constant.

**Type:** int

### PageSetup.PrintHeadings property {#printheadings}

Represents if row and column headings are printed with this page.

**Type:** boolean

### PageSetup.PrintGridlines property {#printgridlines}

Represents if cell gridlines are printed on the page.

**Type:** boolean

### PageSetup.Zoom property {#zoom}

Represents the scaling factor in percent. It should be between 10 and 400.

**Type:** int

### PageSetup.IsAutoFirstPageNumber property {#isautofirstpagenumber}

Indicates whether the first the page number is automatically assigned.

**Type:** boolean

### PageSetup.PrintQuality property {#printquality}

Represents the print quality.

**Type:** int

### PageSetup.PrintCopies property {#printcopies}

Get and sets number of copies to print.

**Type:** int

### PageSetup.IsHFDiffOddEven property {#ishfdiffoddeven}

True means that the header/footer of the odd pages is different with odd pages.

**Type:** boolean

### PageSetup.IsHFDiffFirst property {#ishfdifffirst}

True means that the header/footer of the first page is different with other pages.

**Type:** boolean

### PageSetup.IsHFScaleWithDoc property {#ishfscalewithdoc}

Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

**Type:** boolean

### PageSetup.IsHFAlignMargins property {#ishfalignmargins}

Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

**Type:** boolean

### setHeaderPicture(section, headerPicture) {#setheaderpicture}

Sets an image in the header of a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerPicture | byte[] | Image data. |

**Returns:** Returns Picture object.

### setFooterPicture(section, footerPicture) {#setfooterpicture}

Sets an image in the footer of a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerPicture | byte[] | Image data. |

**Returns:** Returns Picture object.

### setPicture(isFirst, isEven, isHeader, section, imageData) {#setpicture}

Sets an image in the header/footer of a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether setting the picture of first page header/footer. |
| isEven | boolean | Indicates whether setting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether setting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| imageData | byte[] | Image data. |

**Returns:** Returns Picture object.

### getPicture(isHeader, section) (1 of 2) {#getpicture}

Gets the Picture object of the header / footer.

| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | boolean | Indicates whether it is in the header or footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:** Returns Picture object. Returns null if there is no picture.

---

### getPicture(isFirst, isEven, isHeader, section) (2 of 2) {#getpicture-1}

Gets the Picture object of the header / footer.

| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indicates whether getting the picture of first page header/footer. |
| isEven | boolean | Indicates whether getting the picture of even page header/footer. |
| isHeader | boolean | Indicates whether getting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

**Returns:** Returns Picture object.

### copy(source, copyOptions) {#copy}

Copies the setting of the page setup.

| Parameter | Type | Description |
| --- | --- | --- |
| source | PageSetup | The source. |
| copyOptions | CopyOptions | The copy options. |

### setFitToPages(wide, tall) {#setfittopages}

Sets the number of pages the worksheet will be scaled to when it's printed.

| Parameter | Type | Description |
| --- | --- | --- |
| wide | int | Pages wide. |
| tall | int | Pages tall. |

### customPaperSize(width, height) {#custompapersize}

Sets the custom paper size, in unit of inches.

| Parameter | Type | Description |
| --- | --- | --- |
| width | float | The width of the paper. |
| height | float | The height of the paper. |

### clearHeaderFooter() {#clearheaderfooter}

Clears header and footer setting.

### getHeader(section) {#getheader}

Gets a script formatting the header of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

### getCommands(headerFooterScript) {#getcommands}

Gets all commands of header or footer.

| Parameter | Type | Description |
| --- | --- | --- |
| headerFooterScript | String | The header/footer script |

**Returns:** Returns all commands of header or footer.

### getFooter(section) {#getfooter}

Gets a script formatting the footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

### setHeader(section, headerScript) {#setheader}

Sets a script formatting the header of an Excel file.

Script commands: Command Description &P Current page number &N Page count &D Current date &T Current time &A Sheet name &F File name without path &"<FontName>" Font name, for example: &"Arial" &"<FontName>, <FontStyle>" Font name and font style, for example: &"Arial,Bold" &<FontSize> Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. &K<RRGGBB> Font color, for example(RED): &KFF0000 &G Image script For example: "&Arial,Bold&8Header Note"

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### setFooter(section, footerScript) {#setfooter}

Sets a script formatting the footer of an Excel file.

Script commands: Command Description &P Current page number &N Page count &D Current date &T Current time &A Sheet name &F File name without path &"<FontName>" Font name, for example: &"Arial" &"<FontName>, <FontStyle>" Font name and font style, for example: &"Arial,Bold" &<FontSize> Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. &K<RRGGBB> Font color, for example(RED): &KFF0000 &G Image script For example: "&Arial,Bold&8Footer Note"

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### setEvenHeader(section, headerScript) {#setevenheader}

Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### getEvenHeader(section) {#getevenheader}

Gets a script formatting the even header of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

### setEvenFooter(section, footerScript) {#setevenfooter}

Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### getEvenFooter(section) {#getevenfooter}

Gets a script formatting the even footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

### setFirstPageHeader(section, headerScript) {#setfirstpageheader}

Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### getFirstPageHeader(section) {#getfirstpageheader}

Gets a script formatting the first page header of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |

### setFirstPageFooter(section, footerScript) {#setfirstpagefooter}

Sets a script formatting the first page footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### getFirstPageFooter(section) {#getfirstpagefooter}

Gets a script formatting the first page footer of an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
