---
title: "Sparkline"
second_title: "Aspose.Cells för Java API-referens"
description: "En sparkline representerar ett litet diagram eller grafik i en kalkylbladscell som ger en visuell representation av data."
type: docs
url: /sv/java/com.aspose.cells/sparkline/
---

**Inheritance:**
java.lang.Object
```
public class Sparkline
```

En sparkline representerar ett litet diagram eller grafik i en kalkylbladscell som ger en visuell representation av data.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, sheet.getName() + "!A1:D1", false, ca);
 
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         idx = group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         Sparkline line = group.getSparklines().get(idx);
         System.out.println("Saprkline data range: " + line.getDataRange() + ", row: " + line.getRow() + ", column: " + line.getColumn());
         line.toImage("output.png", new ImageOrPrintOptions());
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar kolumnindexet för sparkline. |
| [getDataRange()](#getDataRange--) | Representerar dataområdet för sparkline. |
| [getRow()](#getRow--) | Hämtar radindexet för sparkline. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataRange(String value)](#setDataRange-java.lang.String-) | Representerar dataområdet för sparkline. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Konverterar en sparkline till en bild. |
| [toImage(String fileName, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Konverterar en sparkline till en bild. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Hämtar kolumnindexet för sparkline.

**Returns:**
int
### getDataRange() {#getDataRange--}
```
public String getDataRange()
```


Representerar dataområdet för sparkline.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar radindexet för sparkline.

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




### setDataRange(String value) {#setDataRange-java.lang.String-}
```
public void setDataRange(String value)
```


Representerar dataområdet för sparkline.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Konverterar en sparkline till en bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Bildströmmen. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Bildalternativen. |

### toImage(String fileName, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String fileName, ImageOrPrintOptions options)
```


Konverterar en sparkline till en bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Bildfilens namn. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Bildalternativen |

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

