---
title: "PageSetup"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar sidinställningsbeskrivningen."
type: docs
url: /sv/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Inkapslar objektet som representerar sidinställningsbeskrivningen. PageSetup-objektet innehåller alla sidinställningsalternativ.

**Example**

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Rensar rubrik- och sidfotsinställning. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Kopierar inställningarna för sidinställningen. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Ställer in anpassad pappersstorlek, i tum. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Anger om dokumentets element ska skrivas ut i svartvitt. |
| [getBottomMargin()](#getBottomMargin--) | Anger storleken på den nedre marginalen, i centimeter. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Anger storleken på den nedre marginalen, i tum. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Anger om bladet skrivs ut centrerat horisontellt. |
| [getCenterVertically()](#getCenterVertically--) | Anger om bladet skrivs ut centrerat vertikalt. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Hämtar alla kommandon för rubrik eller sidfot. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Hämtar ett skript som formaterar jämna sidfötter i en Excel-fil. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Hämtar ett skript som formaterar jämna rubriker i en Excel-fil. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Hämtar ett skript som formaterar den första sidfoten i en Excel-fil. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Hämtar ett skript som formaterar den första rubriken i en Excel-fil. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Anger det första sidnumret som ska användas när detta blad skrivs ut. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Anger hur många sidor högt arbetsbladet skalas till när det skrivs ut. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Representerar antalet sidor i bredd som kalkylbladet kommer att skalas till när det skrivs ut. |
| [getFooter(int section)](#getFooter-int-) | Hämtar ett skript som formaterar sidfoten i en Excel‑fil. |
| [getFooterMargin()](#getFooterMargin--) | Representerar avståndet från sidans botten till sidfoten, i enheten centimeter. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Representerar avståndet från sidans botten till sidfoten, i enheten tum. |
| [getHeader(int section)](#getHeader-int-) | Hämtar ett skript som formaterar sidhuvudet i en Excel‑fil. |
| [getHeaderMargin()](#getHeaderMargin--) | Representerar avståndet från sidans topp till sidhuvudet, i enheten centimeter. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Representerar avståndet från sidans topp till sidhuvudet, i enheten tum. |
| [getLeftMargin()](#getLeftMargin--) | Representerar storleken på vänstermarginalen, i enheten centimeter. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Representerar storleken på vänstermarginalen, i enheten tum. |
| [getODSPageBackground()](#getODSPageBackground--) | Hämtar bakgrunden för ODS. |
| [getOrder()](#getOrder--) | Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort kalkylblad skrivs ut. |
| [getOrientation()](#getOrientation--) | Representerar sidans utskriftsorientering. |
| [getPaperHeight()](#getPaperHeight--) | Hämtar papperets höjd i enheten tum, med hänsyn till sidans orientering. |
| [getPaperSize()](#getPaperSize--) | Representerar papperets storlek. |
| [getPaperWidth()](#getPaperWidth--) | Hämtar papperets bredd i enheten tum, med hänsyn till sidans orientering. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Hämtar [Picture](../../com.aspose.cells/picture)-objektet för sidhuvudet / sidfoten. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Hämtar [Picture](../../com.aspose.cells/picture)-objektet för sidhuvudet / sidfoten. |
| [getPrintArea()](#getPrintArea--) | Representerar det område som ska skrivas ut. |
| [getPrintComments()](#getPrintComments--) | Representerar hur kommentarer skrivs ut med bladet. |
| [getPrintCopies()](#getPrintCopies--) | Hämtar antalet kopior som ska skrivas ut. |
| [getPrintDraft()](#getPrintDraft--) | Representerar om bladet kommer att skrivas ut utan grafik. |
| [getPrintErrors()](#getPrintErrors--) | Anger typen av utskriftsfel som visas. |
| [getPrintGridlines()](#getPrintGridlines--) | Representerar om cellrutnät visas på sidan. |
| [getPrintHeadings()](#getPrintHeadings--) | Representerar om rad- och kolumnrubriker skrivs ut på den här sidan. |
| [getPrintQuality()](#getPrintQuality--) | Representerar utskriftskvaliteten. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Representerar de kolumner som innehåller cellerna som ska upprepas på vänster sida av varje sida. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Representerar de rader som innehåller cellerna som ska upprepas högst upp på varje sida. |
| [getPrinterSettings()](#getPrinterSettings--) | Hämtar inställningarna för standardskrivaren. |
| [getRightMargin()](#getRightMargin--) | Representerar storleken på högermarginalen i enheten centimeter. |
| [getRightMarginInch()](#getRightMarginInch--) | Representerar storleken på högermarginalen i enheten tum. |
| [getTopMargin()](#getTopMargin--) | Representerar storleken på övermarginalen i enheten centimeter. |
| [getTopMarginInch()](#getTopMarginInch--) | Representerar storleken på övermarginalen i enheten tum. |
| [getZoom()](#getZoom--) | Representerar skalningsfaktorn i procent. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Anger om sidnumret på den första sidan tilldelas automatiskt. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Anger om pappersstorleken är automatisk. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Anger om sidhuvud- och sidfotsmarginalerna är justerade med sidmarginalerna. |
| [isHFDiffFirst()](#isHFDiffFirst--) | Sant betyder att sidhuvudet/sidfoten på den första sidan är annorlunda än på andra sidor. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | Sant betyder att sidhuvudet/sidfoten på udda sidor är annorlunda än på udda sidor. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Anger om sidhuvud och sidfot skalas med dokumentets skalning. |
| [isPercentScale()](#isPercentScale--) | Om den här egenskapen är falsk styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Anger om sidnumret på den första sidan tilldelas automatiskt. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Anger om dokumentets element ska skrivas ut i svartvitt. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Anger storleken på den nedre marginalen, i centimeter. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Anger storleken på den nedre marginalen, i tum. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Anger om bladet skrivs ut centrerat horisontellt. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Anger om bladet skrivs ut centrerat vertikalt. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Ställer in ett skript som formaterar jämna sidfötter i en Excel-fil. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Ställer in ett skript som formaterar jämna sidhuvuden i en Excel-fil. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Ställer in ett skript som formaterar första sidfoten i en Excel-fil. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Ställer in ett skript som formaterar första sidhuvudet i en Excel-fil. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Anger det första sidnumret som ska användas när detta blad skrivs ut. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Ställer in antalet sidor som arbetsbladet ska skalas till när det skrivs ut. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Anger hur många sidor högt arbetsbladet skalas till när det skrivs ut. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Representerar antalet sidor i bredd som kalkylbladet kommer att skalas till när det skrivs ut. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Ställer in ett skript som formaterar sidfoten i en Excel-fil. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Representerar avståndet från sidans botten till sidfoten, i enheten centimeter. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Representerar avståndet från sidans botten till sidfoten, i enheten tum. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Ställer in en bild i sidfoten på ett arbetsblad. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Anger om sidhuvud- och sidfotsmarginalerna är justerade med sidmarginalerna. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | Sant betyder att sidhuvudet/sidfoten på den första sidan är annorlunda än på andra sidor. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | Sant betyder att sidhuvudet/sidfoten på udda sidor är annorlunda än på udda sidor. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Anger om sidhuvud och sidfot skalas med dokumentets skalning. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Ställer in ett skript som formaterar sidhuvudet i en Excel-fil. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Representerar avståndet från sidans topp till sidhuvudet, i enheten centimeter. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Representerar avståndet från sidans topp till sidhuvudet, i enheten tum. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Ställer in en bild i sidhuvudet på ett arbetsblad. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Representerar storleken på vänstermarginalen, i enheten centimeter. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Representerar storleken på vänstermarginalen, i enheten tum. |
| [setOrder(int value)](#setOrder-int-) | Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort kalkylblad skrivs ut. |
| [setOrientation(int value)](#setOrientation-int-) | Representerar sidans utskriftsorientering. |
| [setPaperSize(int value)](#setPaperSize-int-) | Representerar papperets storlek. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Om den här egenskapen är falsk styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Ställer in en bild i sidhuvudet/sidfoten på ett arbetsblad. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Representerar det område som ska skrivas ut. |
| [setPrintComments(int value)](#setPrintComments-int-) | Representerar hur kommentarer skrivs ut med bladet. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Ställer in antalet kopior att skriva ut. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Representerar om bladet kommer att skrivas ut utan grafik. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Anger typen av utskriftsfel som visas. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Representerar om cellrutnät visas på sidan. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Representerar om rad- och kolumnrubriker skrivs ut på den här sidan. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Representerar utskriftskvaliteten. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Representerar de kolumner som innehåller cellerna som ska upprepas på vänster sida av varje sida. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Representerar de rader som innehåller cellerna som ska upprepas högst upp på varje sida. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Ställer in inställningarna för standardskrivaren. |
| [setRightMargin(double value)](#setRightMargin-double-) | Representerar storleken på högermarginalen i enheten centimeter. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Representerar storleken på högermarginalen i enheten tum. |
| [setTopMargin(double value)](#setTopMargin-double-) | Representerar storleken på övermarginalen i enheten centimeter. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Representerar storleken på övermarginalen i enheten tum. |
| [setZoom(int value)](#setZoom-int-) | Representerar skalningsfaktorn i procent. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Rensar rubrik- och sidfotsinställning.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Kopierar inställningarna för sidinställningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | Källan. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopieringsalternativen. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Ställer in anpassad pappersstorlek, i tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bredd | double | Papirets bredd. |
| höjd | double | Papirets höjd. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Anger om dokumentets element ska skrivas ut i svartvitt.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Anger storleken på den nedre marginalen, i centimeter.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Anger storleken på den nedre marginalen, i tum.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Anger om bladet skrivs ut centrerat horisontellt.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Anger om bladet skrivs ut centrerat vertikalt.

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


Hämtar alla kommandon för rubrik eller sidfot.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| headerFooterScript | java.lang.String | Header/footer‑skriptet |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Returnerar alla kommandon för header eller footer.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Hämtar ett skript som formaterar jämna sidfötter i en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Hämtar ett skript som formaterar jämna rubriker i en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Hämtar ett skript som formaterar den första sidfoten i en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Hämtar ett skript som formaterar den första rubriken i en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Anger det första sidnumret som ska användas när detta blad skrivs ut.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Representerar antalet sidor i höjd som kalkylbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1.

**Remarks**

Du måste sätta FitToPagesWide till noll om du vill få alla rader att passa på en sida.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Representerar antalet sidor i bredd som kalkylbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1.

**Remarks**

Du måste sätta FitToPagesTall till noll om du vill få alla kolumner att passa på en sida.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Hämtar ett skript som formaterar sidfoten i en Excel‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Representerar avståndet från sidans botten till sidfoten, i enheten centimeter.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Representerar avståndet från sidans botten till sidfoten, i enheten tum.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Hämtar ett skript som formaterar sidhuvudet i en Excel‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Representerar avståndet från sidans topp till sidhuvudet, i enheten centimeter.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Representerar avståndet från sidans topp till sidhuvudet, i enheten tum.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Representerar storleken på vänstermarginalen, i enheten centimeter.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Representerar storleken på vänstermarginalen, i enheten tum.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Hämtar bakgrunden för ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort kalkylblad skrivs ut.

Se [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Representerar sidans utskriftsorientering.

Se [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Hämtar papperets höjd i enheten tum, med hänsyn till sidans orientering.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Representerar papperets storlek.

Se [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Hämtar papperets bredd i enheten tum, med hänsyn till sidans orientering.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Hämtar [Picture](../../com.aspose.cells/picture)-objektet för sidhuvudet / sidfoten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isFirst | boolean | Indikerar om bilden av första sidans header/footer hämtas. |
| isEven | boolean | Indikerar om bilden av jämna sidors header/footer hämtas. |
| isHeader | boolean | Indikerar om bilden av header/footer hämtas. |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Hämtar [Picture](../../com.aspose.cells/picture)-objektet för sidhuvudet / sidfoten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isHeader | boolean | Indikerar om det är i headern eller footern. |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Representerar det område som ska skrivas ut.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Representerar hur kommentarer skrivs ut med bladet.

Se [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Hämtar antalet kopior som ska skrivas ut.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Representerar om bladet kommer att skrivas ut utan grafik.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Anger typen av utskriftsfel som visas.

Se [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Representerar om cellrutnät visas på sidan.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Representerar om rad- och kolumnrubriker skrivs ut på den här sidan.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Representerar utskriftskvaliteten.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Representerar de kolumner som innehåller cellerna som ska upprepas på vänster sida av varje sida.

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


Representerar de rader som innehåller cellerna som ska upprepas högst upp på varje sida.

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


Hämtar inställningarna för standardskrivaren.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Representerar storleken på högermarginalen i enheten centimeter.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Representerar storleken på högermarginalen i enheten tum.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Representerar storleken på övermarginalen i enheten centimeter.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Representerar storleken på övermarginalen i enheten tum.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

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


Anger om sidnumret på den första sidan tilldelas automatiskt.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Anger om pappersstorleken är automatisk.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Indikerar om marginalerna för header och footer är justerade med sidans marginaler. Om denna egenskap är sann kommer den vänstra headern och footern att justeras med den vänstra marginalen, och den högra headern och footern att justeras med den högra marginalen. Detta alternativ är aktiverat som standard.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


Sant betyder att sidhuvudet/sidfoten på den första sidan är annorlunda än på andra sidor.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


Sant betyder att sidhuvudet/sidfoten på udda sidor är annorlunda än på udda sidor.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Indikerar om header och footer skalas med dokumentets skalning. Gäller endast för Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Om den här egenskapen är falsk styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas.

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


Anger om sidnumret på den första sidan tilldelas automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Anger om dokumentets element ska skrivas ut i svartvitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Anger storleken på den nedre marginalen, i centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Anger storleken på den nedre marginalen, i tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Anger om bladet skrivs ut centrerat horisontellt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Anger om bladet skrivs ut centrerat vertikalt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Ställer in ett skript som formaterar jämna sidors footer i en Excel‑fil. Påverkar endast i Excel 2007 när IsHFDiffOddEven är sann.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| footerScript | java.lang.String | Script för format av sidfot. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Ställer in ett skript som formaterar det jämna sidhuvudet i en Excel‑fil. Gäller endast i Excel 2007 när IsHFDiffOddEven är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| headerScript | java.lang.String | Script för sidhuvudformat. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Ställer in ett skript som formaterar första sidfoten i en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| footerScript | java.lang.String | Script för format av sidfot. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Ställer in ett skript som formaterar det första sidhuvudet i en Excel‑fil. Gäller endast i Excel 2007 när IsHFDiffFirst är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| headerScript | java.lang.String | Script för sidhuvudformat. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Anger det första sidnumret som ska användas när detta blad skrivs ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Ställer in antalet sidor som arbetsbladet ska skalas till när det skrivs ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bred | int | Sidor breda. |
| hög | int | Sidor höga. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Representerar antalet sidor i höjd som kalkylbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1.

**Remarks**

Du måste sätta FitToPagesWide till noll om du vill få alla rader att passa på en sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Representerar antalet sidor i bredd som kalkylbladet kommer att skalas till när det skrivs ut. Standardvärdet är 1.

**Remarks**

Du måste sätta FitToPagesTall till noll om du vill få alla kolumner att passa på en sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Ställer in ett skript som formaterar sidfoten i en Excel-fil.

**Remarks**

Skriptkommandon:

| Kommando | Beskrivning |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Aktuellt sidnummer\\u9286\\u20ac |
| &N | Sidantal\\u9286\\u20ac |
| &D | Aktuellt datum\\u9286\\u20ac |
| &T | Aktuell tid |
| &A | Bladnamn |
| &F | Filnamn utan sökväg |
| &\"<FontName>\" | Typsnittsnamn, till exempel: &\"Arial\" |
| &\"<FontName>, <FontStyle>\" | Typsnittsnamn och typsnittsstil, till exempel: &\"Arial,Bold\" |
| &<FontSize> | Teckenstorlek. Om detta kommando följs av ett vanligt tal som ska skrivas ut i rubriken, separeras det från teckenhöjden med ett mellanslag. |
| &K<RRGGBB> | Teckenfärg, till exempel(RÖD): &KFF0000 |
| &G | Bildskript |

Till exempel: "&Arial,Bold&8Footer Note"

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| footerScript | java.lang.String | Script för format av sidfot. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Representerar avståndet från sidans botten till sidfoten, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Representerar avståndet från sidans botten till sidfoten, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Ställer in en bild i sidfoten på ett arbetsblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| footerPicture | byte[] | Bilddata. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Indikerar om marginalerna för header och footer är justerade med sidans marginaler. Om denna egenskap är sann kommer den vänstra headern och footern att justeras med den vänstra marginalen, och den högra headern och footern att justeras med den högra marginalen. Detta alternativ är aktiverat som standard.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


Sant betyder att sidhuvudet/sidfoten på den första sidan är annorlunda än på andra sidor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


Sant betyder att sidhuvudet/sidfoten på udda sidor är annorlunda än på udda sidor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Indikerar om header och footer skalas med dokumentets skalning. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Ställer in ett skript som formaterar sidhuvudet i en Excel-fil.

**Remarks**

Skriptkommandon:

| Kommando | Beskrivning |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Aktuellt sidnummer\\u9286\\u20ac |
| &N | Sidantal\\u9286\\u20ac |
| &D | Aktuellt datum\\u9286\\u20ac |
| &T | Aktuell tid |
| &A | Bladnamn |
| &F | Filnamn utan sökväg |
| &\"<FontName>\" | Typsnittsnamn, till exempel: &\"Arial\" |
| &\"<FontName>, <FontStyle>\" | Typsnittsnamn och typsnittsstil, till exempel: &\"Arial,Bold\" |
| &<FontSize> | Teckenstorlek. Om detta kommando följs av ett vanligt tal som ska skrivas ut i rubriken, separeras det från teckenhöjden med ett mellanslag. |
| &K<RRGGBB> | Teckenfärg, till exempel(RÖD): &KFF0000 |
| &G | Bildskript |

Till exempel: "&Arial,Bold&8Header Note"

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| headerScript | java.lang.String | Script för sidhuvudformat. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Representerar avståndet från sidans topp till sidhuvudet, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Representerar avståndet från sidans topp till sidhuvudet, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Ställer in en bild i sidhuvudet på ett arbetsblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| headerPicture | byte[] | Bilddata. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Representerar storleken på vänstermarginalen, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Representerar storleken på vänstermarginalen, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Representerar den ordning som Microsoft Excel använder för att numrera sidor när ett stort kalkylblad skrivs ut.

Se [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Representerar sidans utskriftsorientering.

Se [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Representerar papperets storlek.

Se [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Om den här egenskapen är falsk styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Ställer in en bild i sidhuvudet/sidfoten på ett arbetsblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isFirst | boolean | Anger om bilden för första sidans rubrik/fot ska ställas in. |
| isEven | boolean | Anger om bilden för jämna sidors rubrik/fot ska ställas in. |
| isHeader | boolean | Anger om bilden för rubrik/fot ska ställas in. |
| section | int | 0: Vänster sektion, 1: Mitten sektion, 2: Höger sektion. |
| imageData | byte[] | Bilddata. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Representerar det område som ska skrivas ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Representerar hur kommentarer skrivs ut med bladet.

Se [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Ställer in antalet kopior att skriva ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Representerar om bladet kommer att skrivas ut utan grafik.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Anger typen av utskriftsfel som visas.

Se [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Representerar om cellrutnät visas på sidan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Representerar om rad- och kolumnrubriker skrivs ut på den här sidan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Representerar utskriftskvaliteten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Representerar de kolumner som innehåller cellerna som ska upprepas på vänster sida av varje sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Representerar de rader som innehåller cellerna som ska upprepas högst upp på varje sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Ställer in inställningarna för standardskrivaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Representerar storleken på högermarginalen i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Representerar storleken på högermarginalen i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Representerar storleken på övermarginalen i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Representerar storleken på övermarginalen i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

