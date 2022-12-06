---
title: Sparkline
second_title: Aspose.Cells for Java API Reference
description: A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
type: docs
url: /java/com.aspose.cells/sparkline/
---

**Inheritance:**
java.lang.Object
```
public class Sparkline
```

A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.

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
 
         int idx = sheet.getSparklineGroupCollection().add(com.aspose.cells.SparklineType.LINE, sheet.getName() + "!A1:D1", false, ca);
 
         SparklineGroup group = sheet.getSparklineGroupCollection().get(idx);
         idx = group.getSparklineCollection().add(sheet.getName() + "!A1:D1", 0, 4);
         Sparkline line = group.getSparklineCollection().get(idx);
         System.out.println("Saprkline data range: " + line.getDataRange() + ", row: " + line.getRow() + ", column: " + line.getColumn());
         line.toImage("output.png", new ImageOrPrintOptions());
```
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets the column index of the sparkline. |
| [getDataRange()](#getDataRange--) | Represents the data range of the sparkline. |
| [getRow()](#getRow--) | Gets the row index of the sparkline. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataRange(String value)](#setDataRange-java.lang.String-) | For the description of this property, please see [getDataRange()](../../com.aspose.cells/sparkline\#getDataRange--) |
| [toImage(InputStream stream, ImageOrPrintOptions options)](#toImage-java.io.InputStream-com.aspose.cells.ImageOrPrintOptions-) | Converts a sparkline to an image. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Converts a sparkline to an image. |
| [toImage(String fileName, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Converts a sparkline to an image. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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


Gets the column index of the sparkline.

**Returns:**
int
### getDataRange() {#getDataRange--}
```
public String getDataRange()
```


Represents the data range of the sparkline.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Gets the row index of the sparkline.

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


For the description of this property, please see [getDataRange()](../../com.aspose.cells/sparkline\#getDataRange--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### toImage(InputStream stream, ImageOrPrintOptions options) {#toImage-java.io.InputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(InputStream stream, ImageOrPrintOptions options)
```


Converts a sparkline to an image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The image stream. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | The image options. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Converts a sparkline to an image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The image stream. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | The image options. |

### toImage(String fileName, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String fileName, ImageOrPrintOptions options)
```


Converts a sparkline to an image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The image file name. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | The image options |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

