---
title: "VerticalPageBreak"
second_title: "Aspose.Cells for Java API Referansı"
description: "Dikey sayfa sonunu temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

Dikey sayfa sonunu temsil eden nesneyi kapsüller.

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Dikey sayfa sonunun sütun indeksini alır. |
| [getEndRow()](#getEndRow--) | Dikey sayfa sonunun son satır indeksini alır. |
| [getStartRow()](#getStartRow--) | Dikey sayfa sonunun başlangıç satır indeksini alır. |
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
| Parametre | Tür | Açıklama |
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


Dikey sayfa sonunun sütun indeksini alır.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Dikey sayfa sonunun son satır indeksini alır.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Dikey sayfa sonunun başlangıç satır indeksini alır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

