---
title: "PageSetup"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta la descrizione dell'impostazione della pagina."
type: docs
url: /it/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Incapsula l'oggetto che rappresenta la descrizione dell'impostazione della pagina. L'oggetto PageSetup contiene tutte le opzioni di impostazione della pagina.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Cancella le impostazioni di intestazione e piè di pagina. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Copia le impostazioni dell'impostazione della pagina. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Imposta la dimensione personalizzata della carta, in unità di pollici. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Rappresenta se gli elementi del documento saranno stampati in bianco e nero. |
| [getBottomMargin()](#getBottomMargin--) | Rappresenta la dimensione del margine inferiore, in unità di centimetri. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Rappresenta la dimensione del margine inferiore, in unità di pollici. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Rappresenta se il foglio è stampato centrato orizzontalmente. |
| [getCenterVertically()](#getCenterVertically--) | Rappresenta se il foglio è stampato centrato verticalmente. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Ottiene tutti i comandi dell'intestazione o del piè di pagina. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Ottiene uno script che formatta il piè di pagina pari di un file Excel. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Ottiene uno script che formatta l'intestazione pari di un file Excel. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Ottiene uno script che formatta il piè di pagina della prima pagina di un file Excel. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Ottiene uno script che formatta l'intestazione della prima pagina di un file Excel. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Rappresenta il numero della prima pagina che verrà usato quando questo foglio viene stampato. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando viene stampato. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando viene stampato. |
| [getFooter(int section)](#getFooter-int-) | Ottiene uno script che formatta il piè di pagina di un file Excel. |
| [getFooterMargin()](#getFooterMargin--) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di centimetri. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di pollici. |
| [getHeader(int section)](#getHeader-int-) | Ottiene uno script che formatta l'intestazione di un file Excel. |
| [getHeaderMargin()](#getHeaderMargin--) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di centimetri. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di pollici. |
| [getLeftMargin()](#getLeftMargin--) | Rappresenta la dimensione del margine sinistro, in unità di centimetri. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Rappresenta la dimensione del margine sinistro, in unità di pollici. |
| [getODSPageBackground()](#getODSPageBackground--) | Ottiene lo sfondo di ODS. |
| [getOrder()](#getOrder--) | Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine quando stampa un foglio di lavoro grande. |
| [getOrientation()](#getOrientation--) | Rappresenta l'orientamento di stampa della pagina. |
| [getPaperHeight()](#getPaperHeight--) | Ottiene l'altezza della carta in unità di pollici, considerando l'orientamento della pagina. |
| [getPaperSize()](#getPaperSize--) | Rappresenta le dimensioni della carta. |
| [getPaperWidth()](#getPaperWidth--) | Ottiene la larghezza della carta in unità di pollici, considerando l'orientamento della pagina. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Ottiene l'oggetto [Picture](../../com.aspose.cells/picture) dell'intestazione / piè di pagina. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Ottiene l'oggetto [Picture](../../com.aspose.cells/picture) dell'intestazione / piè di pagina. |
| [getPrintArea()](#getPrintArea--) | Rappresenta l'intervallo da stampare. |
| [getPrintComments()](#getPrintComments--) | Rappresenta il modo in cui i commenti vengono stampati con il foglio. |
| [getPrintCopies()](#getPrintCopies--) | Ottiene il numero di copie da stampare. |
| [getPrintDraft()](#getPrintDraft--) | Rappresenta se il foglio verrà stampato senza grafica. |
| [getPrintErrors()](#getPrintErrors--) | Specifica il tipo di errore di stampa visualizzato. |
| [getPrintGridlines()](#getPrintGridlines--) | Rappresenta se le linee della griglia delle celle vengono stampate sulla pagina. |
| [getPrintHeadings()](#getPrintHeadings--) | Rappresenta se le intestazioni di righe e colonne vengono stampate con questa pagina. |
| [getPrintQuality()](#getPrintQuality--) | Rappresenta la qualità di stampa. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina. |
| [getPrinterSettings()](#getPrinterSettings--) | Ottiene le impostazioni della stampante predefinita. |
| [getRightMargin()](#getRightMargin--) | Rappresenta la dimensione del margine destro, in unità di centimetri. |
| [getRightMarginInch()](#getRightMarginInch--) | Rappresenta la dimensione del margine destro, in unità di pollici. |
| [getTopMargin()](#getTopMargin--) | Rappresenta la dimensione del margine superiore, in unità di centimetri. |
| [getTopMarginInch()](#getTopMarginInch--) | Rappresenta la dimensione del margine superiore, in unità di pollici. |
| [getZoom()](#getZoom--) | Rappresenta il fattore di scala in percentuale. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Indica se il numero della prima pagina viene assegnato automaticamente. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Indica se la dimensione della carta è automatica. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Indica se i margini di intestazione e piè di pagina sono allineati ai margini della pagina. |
| [isHFDiffFirst()](#isHFDiffFirst--) | True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | True indica che l'intestazione/piè di pagina delle pagine dispari è diversa dalle pagine dispari. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Indica se l'intestazione e il piè di pagina sono scalati con la scala del documento. |
| [isPercentScale()](#isPercentScale--) | Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Indica se il numero della prima pagina viene assegnato automaticamente. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Rappresenta se gli elementi del documento saranno stampati in bianco e nero. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Rappresenta la dimensione del margine inferiore, in unità di centimetri. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Rappresenta la dimensione del margine inferiore, in unità di pollici. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Rappresenta se il foglio è stampato centrato orizzontalmente. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Rappresenta se il foglio è stampato centrato verticalmente. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Imposta uno script che formatta il piè di pagina delle pagine pari di un file Excel. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Imposta uno script che formatta l'intestazione delle pagine pari di un file Excel. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Imposta uno script che formatta il piè di pagina della prima pagina di un file Excel. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Imposta uno script che formatta l'intestazione della prima pagina di un file Excel. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Rappresenta il numero della prima pagina che verrà usato quando questo foglio viene stampato. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Imposta il numero di pagine a cui il foglio di lavoro sarà scalato quando viene stampato. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando viene stampato. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando viene stampato. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Imposta uno script che formatta il piè di pagina di un file Excel. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di centimetri. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di pollici. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Imposta un'immagine nel piè di pagina di un foglio di lavoro. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Indica se i margini di intestazione e piè di pagina sono allineati ai margini della pagina. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | True indica che l'intestazione/piè di pagina delle pagine dispari è diversa dalle pagine dispari. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Indica se l'intestazione e il piè di pagina sono scalati con la scala del documento. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Imposta uno script che formatta l'intestazione di un file Excel. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di centimetri. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di pollici. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Imposta un'immagine nell'intestazione di un foglio di lavoro. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Rappresenta la dimensione del margine sinistro, in unità di centimetri. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Rappresenta la dimensione del margine sinistro, in unità di pollici. |
| [setOrder(int value)](#setOrder-int-) | Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine quando stampa un foglio di lavoro grande. |
| [setOrientation(int value)](#setOrientation-int-) | Rappresenta l'orientamento di stampa della pagina. |
| [setPaperSize(int value)](#setPaperSize-int-) | Rappresenta le dimensioni della carta. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Imposta un'immagine nell'intestazione/piè di pagina di un foglio di lavoro. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Rappresenta l'intervallo da stampare. |
| [setPrintComments(int value)](#setPrintComments-int-) | Rappresenta il modo in cui i commenti vengono stampati con il foglio. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Imposta il numero di copie da stampare. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Rappresenta se il foglio verrà stampato senza grafica. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Specifica il tipo di errore di stampa visualizzato. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Rappresenta se le linee della griglia delle celle vengono stampate sulla pagina. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Rappresenta se le intestazioni di righe e colonne vengono stampate con questa pagina. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Rappresenta la qualità di stampa. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Imposta le impostazioni della stampante predefinita. |
| [setRightMargin(double value)](#setRightMargin-double-) | Rappresenta la dimensione del margine destro, in unità di centimetri. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Rappresenta la dimensione del margine destro, in unità di pollici. |
| [setTopMargin(double value)](#setTopMargin-double-) | Rappresenta la dimensione del margine superiore, in unità di centimetri. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Rappresenta la dimensione del margine superiore, in unità di pollici. |
| [setZoom(int value)](#setZoom-int-) | Rappresenta il fattore di scala in percentuale. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Cancella le impostazioni di intestazione e piè di pagina.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Copia le impostazioni dell'impostazione della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | La sorgente. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Le opzioni di copia. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Imposta la dimensione personalizzata della carta, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| larghezza | double | La larghezza della carta. |
| altezza | double | L'altezza della carta. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Rappresenta se gli elementi del documento saranno stampati in bianco e nero.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Rappresenta la dimensione del margine inferiore, in unità di centimetri.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Rappresenta la dimensione del margine inferiore, in unità di pollici.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Rappresenta se il foglio è stampato centrato orizzontalmente.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Rappresenta se il foglio è stampato centrato verticalmente.

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


Ottiene tutti i comandi dell'intestazione o del piè di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| headerFooterScript | java.lang.String | Lo script intestazione/piè di pagina |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Restituisce tutti i comandi dell'intestazione o del piè di pagina.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Ottiene uno script che formatta il piè di pagina pari di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Ottiene uno script che formatta l'intestazione pari di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Ottiene uno script che formatta il piè di pagina della prima pagina di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Ottiene uno script che formatta l'intestazione della prima pagina di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Rappresenta il numero della prima pagina che verrà usato quando questo foglio viene stampato.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando stampato. Il valore predefinito è 1.

**Remarks**

È necessario impostare FitToPagesWide a zero se si desidera adattare tutte le righe su una pagina.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando stampato. Il valore predefinito è 1.

**Remarks**

È necessario impostare FitToPagesTall a zero se si desidera adattare tutte le colonne su una pagina.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Ottiene uno script che formatta il piè di pagina di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di centimetri.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di pollici.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Ottiene uno script che formatta l'intestazione di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di centimetri.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di pollici.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Rappresenta la dimensione del margine sinistro, in unità di centimetri.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Rappresenta la dimensione del margine sinistro, in unità di pollici.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Ottiene lo sfondo di ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine quando stampa un foglio di lavoro grande.

Vedi [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Rappresenta l'orientamento di stampa della pagina.

Vedi [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Ottiene l'altezza della carta in unità di pollici, considerando l'orientamento della pagina.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Rappresenta le dimensioni della carta.

Vedi [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Ottiene la larghezza della carta in unità di pollici, considerando l'orientamento della pagina.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Ottiene l'oggetto [Picture](../../com.aspose.cells/picture) dell'intestazione / piè di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isFirst | boolean | Indica se si sta ottenendo l'immagine dell'intestazione/piè di pagina della prima pagina. |
| isEven | boolean | Indica se si sta ottenendo l'immagine dell'intestazione/piè di pagina delle pagine pari. |
| isHeader | boolean | Indica se ottenere l'immagine dell'intestazione/piè di pagina. |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Ottiene l'oggetto [Picture](../../com.aspose.cells/picture) dell'intestazione / piè di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isHeader | boolean | Indica se si trova nell'intestazione o nel piè di pagina. |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Rappresenta l'intervallo da stampare.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Rappresenta il modo in cui i commenti vengono stampati con il foglio.

Vedi [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Ottiene il numero di copie da stampare.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Rappresenta se il foglio verrà stampato senza grafica.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Specifica il tipo di errore di stampa visualizzato.

Vedi [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Rappresenta se le linee della griglia delle celle vengono stampate sulla pagina.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Rappresenta se le intestazioni di righe e colonne vengono stampate con questa pagina.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Rappresenta la qualità di stampa.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina.

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


Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina.

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


Ottiene le impostazioni della stampante predefinita.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Rappresenta la dimensione del margine destro, in unità di centimetri.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Rappresenta la dimensione del margine destro, in unità di pollici.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Rappresenta la dimensione del margine superiore, in unità di centimetri.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Rappresenta la dimensione del margine superiore, in unità di pollici.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

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


Indica se il numero della prima pagina viene assegnato automaticamente.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Indica se la dimensione della carta è automatica.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Indica se i margini dell'intestazione e del piè di pagina sono allineati ai margini della pagina. Se questa proprietà è vera, l'intestazione e il piè di pagina sinistro saranno allineati al margine sinistro, e quelli destro saranno allineati al margine destro. Questa opzione è abilitata per impostazione predefinita.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


True indica che l'intestazione/piè di pagina delle pagine dispari è diversa dalle pagine dispari.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Indica se l'intestazione e il piè di pagina sono scalati con la scala del documento. Si applica solo a Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro viene scalato.

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


Indica se il numero della prima pagina viene assegnato automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Rappresenta se gli elementi del documento saranno stampati in bianco e nero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Rappresenta la dimensione del margine inferiore, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Rappresenta la dimensione del margine inferiore, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Rappresenta se il foglio è stampato centrato orizzontalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Rappresenta se il foglio è stampato centrato verticalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Imposta uno script che formatta il piè di pagina delle pagine pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è vero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerScript | java.lang.String | Script di formattazione del piè di pagina. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Imposta uno script che formatta l'intestazione delle pagine pari di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffOddEven è vero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerScript | java.lang.String | Script di formattazione dell'intestazione. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Imposta uno script che formatta il piè di pagina della prima pagina di un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerScript | java.lang.String | Script di formattazione del piè di pagina. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Imposta uno script che formatta l'intestazione della prima pagina di un file Excel. Ha effetto solo in Excel 2007 quando IsHFDiffFirst è vero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerScript | java.lang.String | Script di formattazione dell'intestazione. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Rappresenta il numero della prima pagina che verrà usato quando questo foglio viene stampato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Imposta il numero di pagine a cui il foglio di lavoro sarà scalato quando viene stampato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| wide | int | Pagine in larghezza. |
| tall | int | Pagine in altezza. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Rappresenta il numero di pagine in altezza a cui il foglio di lavoro sarà scalato quando stampato. Il valore predefinito è 1.

**Remarks**

È necessario impostare FitToPagesWide a zero se si desidera adattare tutte le righe su una pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando stampato. Il valore predefinito è 1.

**Remarks**

È necessario impostare FitToPagesTall a zero se si desidera adattare tutte le colonne su una pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Imposta uno script che formatta il piè di pagina di un file Excel.

**Remarks**

Comandi script:

| Comando | Descrizione |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Numero di pagina corrente\u9286\u20ac |
| &N | Conteggio pagine\u9286\u20ac |
| &D | Data corrente\u9286\u20ac |
| &T | Ora corrente |
| &A | Nome del foglio |
| &F | Nome file senza percorso |
| &"<FontName>" | Nome del carattere, ad esempio: &"Arial" |
| &"<FontName>, <FontStyle>" | Nome del carattere e stile del carattere, ad esempio: &"Arial,Bold" |
| &<FontSize> | Dimensione del carattere. Se questo comando è seguito da un numero semplice da stampare nell'intestazione, sarà separato dall'altezza del carattere con uno spazio. |
| &K<RRGGBB> | Colore del carattere, ad esempio (ROSSO): &KFF0000 |
| &G | Script immagine |

Ad esempio: "&Arial,Bold&8Footer Note"

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerScript | java.lang.String | Script di formattazione del piè di pagina. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Rappresenta la distanza dal fondo della pagina al piè di pagina, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Imposta un'immagine nel piè di pagina di un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerPicture | byte[] | Dati immagine. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Indica se i margini dell'intestazione e del piè di pagina sono allineati ai margini della pagina. Se questa proprietà è vera, l'intestazione e il piè di pagina sinistro saranno allineati al margine sinistro, e quelli destro saranno allineati al margine destro. Questa opzione è abilitata per impostazione predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


True indica che l'intestazione/piè di pagina della prima pagina è diversa dalle altre pagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


True indica che l'intestazione/piè di pagina delle pagine dispari è diversa dalle pagine dispari.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Indica se l'intestazione e il piè di pagina sono scalati con la scala del documento. Si applica solo a Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Imposta uno script che formatta l'intestazione di un file Excel.

**Remarks**

Comandi script:

| Comando | Descrizione |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Numero di pagina corrente\u9286\u20ac |
| &N | Conteggio pagine\u9286\u20ac |
| &D | Data corrente\u9286\u20ac |
| &T | Ora corrente |
| &A | Nome del foglio |
| &F | Nome file senza percorso |
| &"<FontName>" | Nome del carattere, ad esempio: &"Arial" |
| &"<FontName>, <FontStyle>" | Nome del carattere e stile del carattere, ad esempio: &"Arial,Bold" |
| &<FontSize> | Dimensione del carattere. Se questo comando è seguito da un numero semplice da stampare nell'intestazione, sarà separato dall'altezza del carattere con uno spazio. |
| &K<RRGGBB> | Colore del carattere, ad esempio (ROSSO): &KFF0000 |
| &G | Script immagine |

Ad esempio: "&Arial,Bold&8Header Note"

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerScript | java.lang.String | Script di formattazione dell'intestazione. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Rappresenta la distanza dalla parte superiore della pagina all'intestazione, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Imposta un'immagine nell'intestazione di un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerPicture | byte[] | Dati immagine. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Rappresenta la dimensione del margine sinistro, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Rappresenta la dimensione del margine sinistro, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Rappresenta l'ordine che Microsoft Excel utilizza per numerare le pagine quando stampa un foglio di lavoro grande.

Vedi [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Rappresenta l'orientamento di stampa della pagina.

Vedi [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Rappresenta le dimensioni della carta.

Vedi [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Se questa proprietà è False, le proprietà FitToPagesWide e FitToPagesTall controllano come il foglio di lavoro viene scalato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Imposta un'immagine nell'intestazione/piè di pagina di un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isFirst | boolean | Indica se impostare l'immagine dell'intestazione/piè di pagina della prima pagina. |
| isEven | boolean | Indica se impostare l'immagine dell'intestazione/piè di pagina delle pagine pari. |
| isHeader | boolean | Indica se impostare l'immagine dell'intestazione/piè di pagina. |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| imageData | byte[] | Dati immagine. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Rappresenta l'intervallo da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Rappresenta il modo in cui i commenti vengono stampati con il foglio.

Vedi [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Imposta il numero di copie da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Rappresenta se il foglio verrà stampato senza grafica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Specifica il tipo di errore di stampa visualizzato.

Vedi [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Rappresenta se le linee della griglia delle celle vengono stampate sulla pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Rappresenta se le intestazioni di righe e colonne vengono stampate con questa pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Rappresenta la qualità di stampa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Rappresenta le colonne che contengono le celle da ripetere sul lato sinistro di ogni pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Rappresenta le righe che contengono le celle da ripetere nella parte superiore di ogni pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Imposta le impostazioni della stampante predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Rappresenta la dimensione del margine destro, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Rappresenta la dimensione del margine destro, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Rappresenta la dimensione del margine superiore, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Rappresenta la dimensione del margine superiore, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

