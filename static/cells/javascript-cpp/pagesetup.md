##PageSetup
Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.
## PageSetup class
Encapsulates the object that represents the page setup description. The PageSetup object contains all page setup options.
```javascript
class PageSetup;
```
### Example
```javascript
const { Workbook } = AsposeCells;
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
