---
title: "خط بياني صغير"
second_title: "Aspose.Cells for Java API Reference"
description: "تمثل sparkline مخططًا أو رسمًا صغيرًا في خلية ورقة العمل يوفر تمثيلًا بصريًا للبيانات."
type: docs
url: /ar/java/com.aspose.cells/sparkline/
---

**Inheritance:**
java.lang.Object
```
public class Sparkline
```

تمثل sparkline مخططًا أو رسمًا صغيرًا في خلية ورقة العمل يوفر تمثيلًا بصريًا للبيانات.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على فهرس العمود للخط البياني الصغير. |
| [getDataRange()](#getDataRange--) | يمثل نطاق البيانات للخط البياني الصغير. |
| [getRow()](#getRow--) | يحصل على فهرس الصف للخط البياني الصغير. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataRange(String value)](#setDataRange-java.lang.String-) | يمثل نطاق البيانات للخط البياني الصغير. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | يحوّل الخط البياني الصغير إلى صورة. |
| [toImage(String fileName, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | يحوّل الخط البياني الصغير إلى صورة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على فهرس العمود للخط البياني الصغير.

**Returns:**
int
### getDataRange() {#getDataRange--}
```
public String getDataRange()
```


يمثل نطاق البيانات للخط البياني الصغير.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على فهرس الصف للخط البياني الصغير.

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


يمثل نطاق البيانات للخط البياني الصغير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


يحوّل الخط البياني الصغير إلى صورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الصورة. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | خيارات الصورة. |

### toImage(String fileName, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String fileName, ImageOrPrintOptions options)
```


يحوّل الخط البياني الصغير إلى صورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم ملف الصورة. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | خيارات الصورة |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

