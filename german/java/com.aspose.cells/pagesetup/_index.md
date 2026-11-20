---
title: "PageSetup"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das die Seitensetup‑Beschreibung darstellt."
type: docs
url: /de/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Kapselt das Objekt, das die Seiten-Setup-Beschreibung darstellt. Das PageSetup-Objekt enthält alle Seiten-Setup-Optionen.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Löscht Kopf- und Fußzeileneinstellungen. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Kopiert die Einstellung des PageSetup. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Legt die benutzerdefinierte Papiergröße fest, in Zoll. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Gibt an, ob Elemente des Dokuments in Schwarzweiß gedruckt werden. |
| [getBottomMargin()](#getBottomMargin--) | Gibt die Größe des unteren Randes an, in Zentimetern. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Gibt die Größe des unteren Randes an, in Zoll. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Gibt an, ob das Blatt horizontal zentriert gedruckt wird. |
| [getCenterVertically()](#getCenterVertically--) | Gibt an, ob das Blatt vertikal zentriert gedruckt wird. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Liefert alle Befehle von Kopf- oder Fußzeile. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Liefert ein Skript, das die gerade Fußzeile einer Excel-Datei formatiert. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Liefert ein Skript, das die gerade Kopfzeile einer Excel-Datei formatiert. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Liefert ein Skript, das die Fußzeile der ersten Seite einer Excel-Datei formatiert. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Liefert ein Skript, das die Kopfzeile der ersten Seite einer Excel-Datei formatiert. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Stellt die erste Seitenzahl dar, die beim Drucken dieses Blatts verwendet wird. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Stellt die Anzahl der Seiten in der Höhe dar, auf die das Arbeitsblatt beim Drucken skaliert wird. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Stellt die Anzahl der Seiten in der Breite dar, auf die das Arbeitsblatt beim Drucken skaliert wird. |
| [getFooter(int section)](#getFooter-int-) | Ruft ein Skript ab, das die Fußzeile einer Excel-Datei formatiert. |
| [getFooterMargin()](#getFooterMargin--) | Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zentimetern dar. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zoll dar. |
| [getHeader(int section)](#getHeader-int-) | Ruft ein Skript ab, das die Kopfzeile einer Excel-Datei formatiert. |
| [getHeaderMargin()](#getHeaderMargin--) | Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zentimetern dar. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zoll dar. |
| [getLeftMargin()](#getLeftMargin--) | Stellt die Größe des linken Randes in Zentimetern dar. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Stellt die Größe des linken Randes in Zoll dar. |
| [getODSPageBackground()](#getODSPageBackground--) | Ruft den Hintergrund von ODS ab. |
| [getOrder()](#getOrder--) | Stellt die Reihenfolge dar, die Microsoft Excel verwendet, um Seiten beim Drucken eines großen Arbeitsblatts zu nummerieren. |
| [getOrientation()](#getOrientation--) | Stellt die Druckorientierung der Seite dar. |
| [getPaperHeight()](#getPaperHeight--) | Ruft die Höhe des Papiers in Zoll ab, berücksichtigt die Seitenorientierung. |
| [getPaperSize()](#getPaperSize--) | Stellt die Papiergröße dar. |
| [getPaperWidth()](#getPaperWidth--) | Ruft die Breite des Papiers in Zoll ab, berücksichtigt die Seitenorientierung. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Ruft das [Picture](../../com.aspose.cells/picture)-Objekt der Kopf- / Fußzeile ab. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Ruft das [Picture](../../com.aspose.cells/picture)-Objekt der Kopf- / Fußzeile ab. |
| [getPrintArea()](#getPrintArea--) | Stellt den zu druckenden Bereich dar. |
| [getPrintComments()](#getPrintComments--) | Stellt dar, wie Kommentare mit dem Blatt gedruckt werden. |
| [getPrintCopies()](#getPrintCopies--) | Ruft die Anzahl der zu druckenden Kopien ab. |
| [getPrintDraft()](#getPrintDraft--) | Stellt dar, ob das Blatt ohne Grafiken gedruckt wird. |
| [getPrintErrors()](#getPrintErrors--) | Gibt den Typ des angezeigten Druckfehlers an. |
| [getPrintGridlines()](#getPrintGridlines--) | Stellt dar, ob Zellgitternetzlinien auf der Seite gedruckt werden. |
| [getPrintHeadings()](#getPrintHeadings--) | Stellt dar, ob Zeilen- und Spaltenüberschriften mit dieser Seite gedruckt werden. |
| [getPrintQuality()](#getPrintQuality--) | Stellt die Druckqualität dar. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Stellt die Spalten dar, die die Zellen enthalten, die auf der linken Seite jeder Seite wiederholt werden. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Stellt die Zeilen dar, die die Zellen enthalten, die oben auf jeder Seite wiederholt werden. |
| [getPrinterSettings()](#getPrinterSettings--) | Ruft die Einstellungen des Standarddruckers ab. |
| [getRightMargin()](#getRightMargin--) | Stellt die Größe des rechten Randes in Zentimetern dar. |
| [getRightMarginInch()](#getRightMarginInch--) | Stellt die Größe des rechten Randes in Zoll dar. |
| [getTopMargin()](#getTopMargin--) | Stellt die Größe des oberen Randes in Zentimetern dar. |
| [getTopMarginInch()](#getTopMarginInch--) | Stellt die Größe des oberen Randes in Zoll dar. |
| [getZoom()](#getZoom--) | Stellt den Skalierungsfaktor in Prozent dar. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Gibt an, ob die erste Seitenzahl automatisch zugewiesen wird. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Gibt an, ob die Papiergröße automatisch ist. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Gibt an, ob Kopf- und Fußzeilenränder mit den Seitenrändern ausgerichtet sind. |
| [isHFDiffFirst()](#isHFDiffFirst--) | True bedeutet, dass die Kopf-/Fußzeile der ersten Seite von den anderen Seiten abweicht. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | True bedeutet, dass die Kopf-/Fußzeile der ungeraden Seiten von den ungeraden Seiten abweicht. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Gibt an, ob Kopf- und Fußzeile mit der Dokumentskalierung skaliert werden. |
| [isPercentScale()](#isPercentScale--) | Wenn diese Eigenschaft False ist, steuern die Eigenschaften FitToPagesWide und FitToPagesTall, wie das Arbeitsblatt skaliert wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Gibt an, ob die erste Seitenzahl automatisch zugewiesen wird. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Gibt an, ob Elemente des Dokuments in Schwarzweiß gedruckt werden. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Gibt die Größe des unteren Randes an, in Zentimetern. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Gibt die Größe des unteren Randes an, in Zoll. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Gibt an, ob das Blatt horizontal zentriert gedruckt wird. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Gibt an, ob das Blatt vertikal zentriert gedruckt wird. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Legt ein Skript fest, das die Fußzeile der geraden Seiten einer Excel-Datei formatiert. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Legt ein Skript fest, das die Kopfzeile der geraden Seiten einer Excel-Datei formatiert. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Legt ein Skript fest, das die Fußzeile der ersten Seite einer Excel-Datei formatiert. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Legt ein Skript fest, das die Kopfzeile der ersten Seite einer Excel-Datei formatiert. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Stellt die erste Seitenzahl dar, die beim Drucken dieses Blatts verwendet wird. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Legt die Anzahl der Seiten fest, auf die das Arbeitsblatt beim Drucken skaliert wird. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Stellt die Anzahl der Seiten in der Höhe dar, auf die das Arbeitsblatt beim Drucken skaliert wird. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Stellt die Anzahl der Seiten in der Breite dar, auf die das Arbeitsblatt beim Drucken skaliert wird. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Legt ein Skript fest, das die Fußzeile einer Excel-Datei formatiert. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zentimetern dar. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zoll dar. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Fügt ein Bild in die Fußzeile eines Arbeitsblatts ein. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Gibt an, ob Kopf- und Fußzeilenränder mit den Seitenrändern ausgerichtet sind. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | True bedeutet, dass die Kopf-/Fußzeile der ersten Seite von den anderen Seiten abweicht. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | True bedeutet, dass die Kopf-/Fußzeile der ungeraden Seiten von den ungeraden Seiten abweicht. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Gibt an, ob Kopf- und Fußzeile mit der Dokumentskalierung skaliert werden. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Legt ein Skript fest, das die Kopfzeile einer Excel-Datei formatiert. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zentimetern dar. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zoll dar. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Fügt ein Bild in die Kopfzeile eines Arbeitsblatts ein. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Stellt die Größe des linken Randes in Zentimetern dar. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Stellt die Größe des linken Randes in Zoll dar. |
| [setOrder(int value)](#setOrder-int-) | Stellt die Reihenfolge dar, die Microsoft Excel verwendet, um Seiten beim Drucken eines großen Arbeitsblatts zu nummerieren. |
| [setOrientation(int value)](#setOrientation-int-) | Stellt die Druckorientierung der Seite dar. |
| [setPaperSize(int value)](#setPaperSize-int-) | Stellt die Papiergröße dar. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Wenn diese Eigenschaft False ist, steuern die Eigenschaften FitToPagesWide und FitToPagesTall, wie das Arbeitsblatt skaliert wird. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Fügt ein Bild in die Kopf-/Fußzeile eines Arbeitsblatts ein. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Stellt den zu druckenden Bereich dar. |
| [setPrintComments(int value)](#setPrintComments-int-) | Stellt dar, wie Kommentare mit dem Blatt gedruckt werden. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Legt die Anzahl der zu druckenden Kopien fest. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Stellt dar, ob das Blatt ohne Grafiken gedruckt wird. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Gibt den Typ des angezeigten Druckfehlers an. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Stellt dar, ob Zellgitternetzlinien auf der Seite gedruckt werden. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Stellt dar, ob Zeilen- und Spaltenüberschriften mit dieser Seite gedruckt werden. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Stellt die Druckqualität dar. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Stellt die Spalten dar, die die Zellen enthalten, die auf der linken Seite jeder Seite wiederholt werden. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Stellt die Zeilen dar, die die Zellen enthalten, die oben auf jeder Seite wiederholt werden. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Legt die Einstellungen des Standarddruckers fest. |
| [setRightMargin(double value)](#setRightMargin-double-) | Stellt die Größe des rechten Randes in Zentimetern dar. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Stellt die Größe des rechten Randes in Zoll dar. |
| [setTopMargin(double value)](#setTopMargin-double-) | Stellt die Größe des oberen Randes in Zentimetern dar. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Stellt die Größe des oberen Randes in Zoll dar. |
| [setZoom(int value)](#setZoom-int-) | Stellt den Skalierungsfaktor in Prozent dar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Löscht Kopf- und Fußzeileneinstellungen.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Kopiert die Einstellung des PageSetup.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | Die Quelle. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Die Kopieroptionen. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Legt die benutzerdefinierte Papiergröße fest, in Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Breite | double | Die Breite des Papiers. |
| Höhe | double | Die Höhe des Papiers. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Gibt an, ob Elemente des Dokuments in Schwarzweiß gedruckt werden.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Gibt die Größe des unteren Randes an, in Zentimetern.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Gibt die Größe des unteren Randes an, in Zoll.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Gibt an, ob das Blatt horizontal zentriert gedruckt wird.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Gibt an, ob das Blatt vertikal zentriert gedruckt wird.

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


Liefert alle Befehle von Kopf- oder Fußzeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| headerFooterScript | java.lang.String | Das Header/Footer‑Skript |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Gibt alle Befehle des Headers oder Footers zurück.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Liefert ein Skript, das die gerade Fußzeile einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Liefert ein Skript, das die gerade Kopfzeile einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Liefert ein Skript, das die Fußzeile der ersten Seite einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Liefert ein Skript, das die Kopfzeile der ersten Seite einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Stellt die erste Seitenzahl dar, die beim Drucken dieses Blatts verwendet wird.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Gibt die Anzahl der Seiten in der Höhe an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1.

**Remarks**

Sie müssen FitToPagesWide auf Null setzen, wenn Sie alle Zeilen auf einer Seite anpassen möchten.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Gibt die Anzahl der Seiten in der Breite an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1.

**Remarks**

Sie müssen FitToPagesTall auf Null setzen, wenn Sie alle Spalten auf einer Seite anpassen möchten.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Ruft ein Skript ab, das die Fußzeile einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zentimetern dar.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zoll dar.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Ruft ein Skript ab, das die Kopfzeile einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zentimetern dar.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zoll dar.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Stellt die Größe des linken Randes in Zentimetern dar.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Stellt die Größe des linken Randes in Zoll dar.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Ruft den Hintergrund von ODS ab.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Stellt die Reihenfolge dar, die Microsoft Excel verwendet, um Seiten beim Drucken eines großen Arbeitsblatts zu nummerieren.

Siehe [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Stellt die Druckorientierung der Seite dar.

Siehe [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Ruft die Höhe des Papiers in Zoll ab, berücksichtigt die Seitenorientierung.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Stellt die Papiergröße dar.

Siehe [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Ruft die Breite des Papiers in Zoll ab, berücksichtigt die Seitenorientierung.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Ruft das [Picture](../../com.aspose.cells/picture)-Objekt der Kopf- / Fußzeile ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isFirst | boolean | Gibt an, ob das Bild des Headers/Footers der ersten Seite abgerufen wird. |
| isEven | boolean | Gibt an, ob das Bild des Headers/Footers einer geraden Seite abgerufen wird. |
| isHeader | boolean | Gibt an, ob das Bild des Headers/Footers abgerufen wird. |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Ruft das [Picture](../../com.aspose.cells/picture)-Objekt der Kopf- / Fußzeile ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isHeader | boolean | Gibt an, ob es sich im Header oder Footer befindet. |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Stellt den zu druckenden Bereich dar.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Stellt dar, wie Kommentare mit dem Blatt gedruckt werden.

Siehe [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Ruft die Anzahl der zu druckenden Kopien ab.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Stellt dar, ob das Blatt ohne Grafiken gedruckt wird.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Gibt den Typ des angezeigten Druckfehlers an.

Siehe [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Stellt dar, ob Zellgitternetzlinien auf der Seite gedruckt werden.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Stellt dar, ob Zeilen- und Spaltenüberschriften mit dieser Seite gedruckt werden.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Stellt die Druckqualität dar.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Stellt die Spalten dar, die die Zellen enthalten, die auf der linken Seite jeder Seite wiederholt werden.

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


Stellt die Zeilen dar, die die Zellen enthalten, die oben auf jeder Seite wiederholt werden.

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


Ruft die Einstellungen des Standarddruckers ab.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Stellt die Größe des rechten Randes in Zentimetern dar.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Stellt die Größe des rechten Randes in Zoll dar.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Stellt die Größe des oberen Randes in Zentimetern dar.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Stellt die Größe des oberen Randes in Zoll dar.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Gibt den Skalierungsfaktor in Prozent an. Er sollte zwischen 10 und 400 liegen.

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


Gibt an, ob die erste Seitenzahl automatisch zugewiesen wird.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Gibt an, ob die Papiergröße automatisch ist.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Gibt an, ob die Kopf- und Fußzeilenränder mit den Seitenrändern ausgerichtet sind. Ist diese Eigenschaft wahr, werden die linke Kopf‑ und Fußzeile am linken Rand und die rechte Kopf‑ und Fußzeile am rechten Rand ausgerichtet. Diese Option ist standardmäßig aktiviert.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


True bedeutet, dass die Kopf-/Fußzeile der ersten Seite von den anderen Seiten abweicht.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


True bedeutet, dass die Kopf-/Fußzeile der ungeraden Seiten von den ungeraden Seiten abweicht.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Gibt an, ob Kopf- und Fußzeile mit der Dokumentskalierung skaliert werden. Gilt nur für Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Wenn diese Eigenschaft False ist, steuern die Eigenschaften FitToPagesWide und FitToPagesTall, wie das Arbeitsblatt skaliert wird.

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


Gibt an, ob die erste Seitenzahl automatisch zugewiesen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Gibt an, ob Elemente des Dokuments in Schwarzweiß gedruckt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Gibt die Größe des unteren Randes an, in Zentimetern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Gibt die Größe des unteren Randes an, in Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Gibt an, ob das Blatt horizontal zentriert gedruckt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Gibt an, ob das Blatt vertikal zentriert gedruckt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Legt ein Skript fest, das die Fußzeile der geraden Seite einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffOddEven true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| footerScript | java.lang.String | Fußzeilenformat‑Skript. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Legt ein Skript fest, das die Kopfzeile der geraden Seite einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffOddEven true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| headerScript | java.lang.String | Kopfzeilenformat‑Skript. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Legt ein Skript fest, das die Fußzeile der ersten Seite einer Excel-Datei formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| footerScript | java.lang.String | Fußzeilenformat‑Skript. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Legt ein Skript fest, das die Kopfzeile der ersten Seite einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffFirst true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| headerScript | java.lang.String | Kopfzeilenformat‑Skript. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Stellt die erste Seitenzahl dar, die beim Drucken dieses Blatts verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Legt die Anzahl der Seiten fest, auf die das Arbeitsblatt beim Drucken skaliert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| wide | int | Seiten breit. |
| tall | int | Seiten hoch. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Gibt die Anzahl der Seiten in der Höhe an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1.

**Remarks**

Sie müssen FitToPagesWide auf Null setzen, wenn Sie alle Zeilen auf einer Seite anpassen möchten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Gibt die Anzahl der Seiten in der Breite an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1.

**Remarks**

Sie müssen FitToPagesTall auf Null setzen, wenn Sie alle Spalten auf einer Seite anpassen möchten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Legt ein Skript fest, das die Fußzeile einer Excel-Datei formatiert.

**Remarks**

Skriptbefehle:

| Befehl | Beschreibung |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Aktuelle Seitenzahl\u9286\u20ac |
| &N | Seitenanzahl\u9286\u20ac |
| &D | Aktuelles Datum\u9286\u20ac |
| &T | Aktuelle Uhrzeit |
| &A | Blattname |
| &F | Dateiname ohne Pfad |
| &"<FontName>" | Schriftname, zum Beispiel: &"Arial" |
| &"<FontName>, <FontStyle>" | Schriftname und Schriftstil, zum Beispiel: &"Arial,Bold" |
| &<FontSize> | Schriftgröße. Wenn diesem Befehl eine einfache Zahl folgt, die in der Kopfzeile gedruckt werden soll, wird sie durch ein Leerzeichen vom Schriftgrad getrennt. |
| &K<RRGGBB> | Schriftfarbe, zum Beispiel (ROT): &KFF0000 |
| &G | Bildskript |

Zum Beispiel: "&Arial,Bold&8Footer Note"

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| footerScript | java.lang.String | Fußzeilenformat‑Skript. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Stellt den Abstand vom unteren Rand der Seite zur Fußzeile in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Fügt ein Bild in die Fußzeile eines Arbeitsblatts ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| footerPicture | byte[] | Bilddaten. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Gibt an, ob die Kopf- und Fußzeilenränder mit den Seitenrändern ausgerichtet sind. Ist diese Eigenschaft wahr, werden die linke Kopf‑ und Fußzeile am linken Rand und die rechte Kopf‑ und Fußzeile am rechten Rand ausgerichtet. Diese Option ist standardmäßig aktiviert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


True bedeutet, dass die Kopf-/Fußzeile der ersten Seite von den anderen Seiten abweicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


True bedeutet, dass die Kopf-/Fußzeile der ungeraden Seiten von den ungeraden Seiten abweicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Gibt an, ob Kopf- und Fußzeile mit der Dokumentskalierung skaliert werden. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Legt ein Skript fest, das die Kopfzeile einer Excel-Datei formatiert.

**Remarks**

Skriptbefehle:

| Befehl | Beschreibung |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Aktuelle Seitenzahl\u9286\u20ac |
| &N | Seitenanzahl\u9286\u20ac |
| &D | Aktuelles Datum\u9286\u20ac |
| &T | Aktuelle Uhrzeit |
| &A | Blattname |
| &F | Dateiname ohne Pfad |
| &"<FontName>" | Schriftname, zum Beispiel: &"Arial" |
| &"<FontName>, <FontStyle>" | Schriftname und Schriftstil, zum Beispiel: &"Arial,Bold" |
| &<FontSize> | Schriftgröße. Wenn diesem Befehl eine einfache Zahl folgt, die in der Kopfzeile gedruckt werden soll, wird sie durch ein Leerzeichen vom Schriftgrad getrennt. |
| &K<RRGGBB> | Schriftfarbe, zum Beispiel (ROT): &KFF0000 |
| &G | Bildskript |

Zum Beispiel: "&Arial,Bold&8Header Note"

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| headerScript | java.lang.String | Kopfzeilenformat‑Skript. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Stellt den Abstand vom oberen Rand der Seite zur Kopfzeile in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Fügt ein Bild in die Kopfzeile eines Arbeitsblatts ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| headerPicture | byte[] | Bilddaten. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Stellt die Größe des linken Randes in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Stellt die Größe des linken Randes in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Stellt die Reihenfolge dar, die Microsoft Excel verwendet, um Seiten beim Drucken eines großen Arbeitsblatts zu nummerieren.

Siehe [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Stellt die Druckorientierung der Seite dar.

Siehe [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Stellt die Papiergröße dar.

Siehe [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Wenn diese Eigenschaft False ist, steuern die Eigenschaften FitToPagesWide und FitToPagesTall, wie das Arbeitsblatt skaliert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Fügt ein Bild in die Kopf-/Fußzeile eines Arbeitsblatts ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isFirst | boolean | Gibt an, ob das Bild der ersten Seitenkopf-/fußzeile festgelegt wird. |
| isEven | boolean | Gibt an, ob das Bild der geraden Seitenkopf-/fußzeile festgelegt wird. |
| isHeader | boolean | Gibt an, ob das Bild der Kopf-/fußzeile festgelegt wird. |
| Abschnitt | int | 0: Linker Abschnitt, 1: Zentraler Abschnitt, 2: Rechter Abschnitt. |
| imageData | byte[] | Bilddaten. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Stellt den zu druckenden Bereich dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Stellt dar, wie Kommentare mit dem Blatt gedruckt werden.

Siehe [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Legt die Anzahl der zu druckenden Kopien fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Stellt dar, ob das Blatt ohne Grafiken gedruckt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Gibt den Typ des angezeigten Druckfehlers an.

Siehe [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Stellt dar, ob Zellgitternetzlinien auf der Seite gedruckt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Stellt dar, ob Zeilen- und Spaltenüberschriften mit dieser Seite gedruckt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Stellt die Druckqualität dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Stellt die Spalten dar, die die Zellen enthalten, die auf der linken Seite jeder Seite wiederholt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Stellt die Zeilen dar, die die Zellen enthalten, die oben auf jeder Seite wiederholt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Legt die Einstellungen des Standarddruckers fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Stellt die Größe des rechten Randes in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Stellt die Größe des rechten Randes in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Stellt die Größe des oberen Randes in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Stellt die Größe des oberen Randes in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Gibt den Skalierungsfaktor in Prozent an. Er sollte zwischen 10 und 400 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

