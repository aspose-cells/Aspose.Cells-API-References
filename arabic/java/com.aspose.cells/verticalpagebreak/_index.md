---
title: "VerticalPageBreak"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل فاصل صفحة عمودي."
type: docs
url: /ar/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

يغلف الكائن الذي يمثل فاصل صفحة عمودي.

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على فهرس العمود لفاصل الصفحة العمودي. |
| [getEndRow()](#getEndRow--) | يحصل على فهرس الصف النهائي لفاصل الصفحة العمودي. |
| [getStartRow()](#getStartRow--) | يحصل على فهرس الصف الابتدائي لفاصل الصفحة العمودي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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


يحصل على فهرس العمود لفاصل الصفحة العمودي.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


يحصل على فهرس الصف النهائي لفاصل الصفحة العمودي.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


يحصل على فهرس الصف الابتدائي لفاصل الصفحة العمودي.

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

