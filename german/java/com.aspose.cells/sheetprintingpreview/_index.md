---
title: "SheetPrintingPreview"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Druckvorschau des Arbeitsblatts."
type: docs
url: /de/java/com.aspose.cells/sheetprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class SheetPrintingPreview
```

Druckvorschau des Arbeitsblatts.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)](#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | Der Aufbau von SheetPrintingPreview |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Ermittle die Gesamtseitenzahl dieses Arbeitsblatts |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options) {#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```


Der Aufbau von SheetPrintingPreview

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Gib an, welches Tabellenblatt gedruckt werden soll. |
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


Ermittle die Gesamtseitenzahl dieses Arbeitsblatts

**Example**

Der folgende Code zeigt den schnellsten Weg, die Seitenzahl eines Arbeitsblatts zu ermitteln.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(workbook.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in worksheet.
         System.out.println(sheetPrintingPreview.getEvaluatedPageCount());
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

