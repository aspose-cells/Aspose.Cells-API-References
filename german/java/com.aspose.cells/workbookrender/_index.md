---
title: "WorkbookRender"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Arbeitsmappen-Darstellung dar."
type: docs
url: /de/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Stellt ein Workbook-Rendering dar. Der Konstruktor dieser Klasse muss nach der Änderung von Seitenlayout und Zellenstil verwendet werden.

**Remarks**
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | Der Aufbau von WorkbookRender |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [dispose()](#dispose--) | Gibt Ressourcen frei, die für das Rendering erstellt und verwendet wurden. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Liefert die Gesamtseitenzahl des Arbeitsbuchs. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Rendern einer bestimmten Seite in einen Stream. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Rendern einer bestimmten Seite in einen Stream. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Rendern einer bestimmten Seite in eine Datei. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Rendern des gesamten Arbeitsbuchs als TIFF-Bild in einen Stream. |
| [toImage(String filename)](#toImage-java.lang.String-) | Rendern des gesamten Arbeitsbuchs als TIFF-Bild in eine Datei. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Rendern des Arbeitsbuchs zum Drucker |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Rendern des Arbeitsbuchs zum Drucker |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Rendern des Arbeitsbuchs zum Drucker |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


Der Aufbau von WorkbookRender

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Gibt an, welches Arbeitsbuch gerendert werden soll. |
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


Liefert die Gesamtseitenzahl des Arbeitsbuchs.

**Returns:**
int
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

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageIndex | int | geben Sie an, welche Seite konvertiert werden soll |
| fileName | java.lang.String | Dateiname des Ausgabebildes |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Rendern des gesamten Arbeitsbuchs als TIFF-Bild in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | der Stream des Ausgabebildes |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Rendern des gesamten Arbeitsbuchs als TIFF-Bild in eine Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | java.lang.String | der Dateiname des Ausgabebildes |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Rendern des Arbeitsbuchs zum Drucker

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Rendern des Arbeitsbuchs zum Drucker

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen ToPrinter(string PrinterName) und ImageOrPrintOptions.PageIndex, PageCount, um die erste Seite und die Anzahl der zu druckenden Seiten festzulegen. Diese Eigenschaft wird 12 Monate später, seit Dezember 2021, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | der Name des Druckers, zum Beispiel: "Microsoft Office Document Image Writer" |
| printPageIndex | int | der nullbasierte Index der ersten zu druckenden Seite, er muss im Bereich [0, WorkbookRender.PageCount-1] liegen |
| printPageCount | int | die Anzahl der zu druckenden Seiten, sie muss größer als null sein |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Rendern des Arbeitsbuchs zum Drucker

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

