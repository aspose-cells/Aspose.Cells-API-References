---
title: "WorkbookPrintingPreview"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Arbeitsmappen-Druckvorschau."
type: docs
url: /de/java/com.aspose.cells/workbookprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookPrintingPreview
```

Arbeitsmappen-Druckvorschau.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)](#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | Der Aufbau von WorkbookPrintingPreview |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Ermitteln Sie die Gesamtseitenzahl dieses Arbeitsbuchs |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options) {#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```


Der Aufbau von WorkbookPrintingPreview

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Geben Sie an, welches Arbeitsbuch gedruckt werden soll. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions enthält einige Eigenschaften der Ausgabe |

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
### getEvaluatedPageCount() {#getEvaluatedPageCount--}
```
public int getEvaluatedPageCount()
```


Ermitteln Sie die Gesamtseitenzahl dieses Arbeitsbuchs

**Example**

Der folgende Code zeigt den schnellsten Weg, die Seitenzahl eines Arbeitsbuchs zu erhalten.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in workbook.
         System.out.println(workbookPrintingPreview.getEvaluatedPageCount());
```

**Returns:**
int
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

