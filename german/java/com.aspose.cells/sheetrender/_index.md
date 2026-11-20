---
title: "SheetRender"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Arbeitsblatt‑Render dar, das ein Arbeitsblatt in verschiedene Bilder wie BMP PNG JPEG TIFF.. rendern kann."
type: docs
url: /de/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Stellt ein Arbeitsblatt‑Render dar, das ein Arbeitsblatt in verschiedene Bilder wie (BMP, PNG, JPEG, TIFF..) rendern kann. Der Konstruktor dieser Klasse muss nach Änderungen an pagesetup, cell style verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | Der Konstruktor von SheetRender benötigt worksheet und ImageOrPrintOptions als params |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [dispose()](#dispose--) | Gibt Ressourcen frei, die für das Rendering erstellt und verwendet wurden. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Liefert die Gesamtseitenzahl des aktuellen Arbeitsblatts. |
| [getPageScale()](#getPageScale--) | Liefert die berechnete Seitenskalierung des Blatts. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Rendern einer bestimmten Seite in einen Stream. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Rendern einer bestimmten Seite in einen Stream. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Rendern einer bestimmten Seite in eine Datei. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Arbeitsblatt zum Drucker rendern |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Arbeitsblatt zum Drucker rendern |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Arbeitsblatt zum Drucker rendern |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Ganzes Arbeitsblatt als Tiff-Bild in einen Stream rendern. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


Der Konstruktor von SheetRender benötigt worksheet und ImageOrPrintOptions als params

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Gibt an, welche Tabelle gerendert werden soll. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions enthält einige Eigenschaften des Ausgabebildes |

### dispose() {#dispose--}
```
public void dispose()
```


Gibt Ressourcen frei, die für das Rendering erstellt und verwendet wurden.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Liefert die Gesamtseitenzahl des aktuellen Arbeitsblatts.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Liefert die berechnete Seitenskalierung des Blatts. Gibt die eingestellte Skalierung zurück, wenn [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) gesetzt ist. Andernfalls wird die berechnete Skalierung gemäß [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) und [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--) zurückgegeben.

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Ermittelt die Seitengröße in Zoll des Ausgabebildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | int | Der Seitenindex ist nullbasiert. |

**Returns:**
float[] – Bildgröße, [0] für Breite und [1] für Höhe
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


Rendern einer bestimmten Seite in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | int | geben Sie an, welche Seite konvertiert werden soll |
| stream | java.io.InputStream | der Stream des Ausgabebildes |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Rendern einer bestimmten Seite in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | int | geben Sie an, welche Seite konvertiert werden soll |
| stream | java.io.OutputStream | der Stream des Ausgabebildes |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Rendern einer bestimmten Seite in eine Datei.

**Example**

Der folgende Code gibt die erste Seite des ersten Blatts als PNG-Bild aus.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | int | geben Sie an, welche Seite konvertiert werden soll |
| fileName | java.lang.String | Dateiname des Ausgabebildes |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Arbeitsblatt zum Drucker rendern

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Arbeitsblatt zum Drucker rendern

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen ToPrinter(string PrinterName) und ImageOrPrintOptions.PageIndex, PageCount, um die erste Seite und die Anzahl der zu druckenden Seiten festzulegen. Diese Eigenschaft wird 12 Monate später, seit Dezember 2021, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer" |
| printPageIndex | int | Der nullbasierte Index der ersten zu druckenden Seite, er muss im Bereich [0, SheetRender.PageCount-1] liegen. |
| printPageCount | int | die Anzahl der zu druckenden Seiten, sie muss größer als null sein |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Arbeitsblatt zum Drucker rendern

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | setzen Sie den Namen des Druckauftrags |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Ganzes Arbeitsblatt als Tiff-Bild in einen Stream rendern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | der Stream des Ausgabebildes |

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

