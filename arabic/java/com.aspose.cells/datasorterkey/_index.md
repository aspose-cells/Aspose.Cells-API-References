---
title: "DataSorterKey"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل المفتاح لـ DataSorter."
type: docs
url: /ar/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

يمثل المفتاح لـ DataSorter.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يحصل على اللون المرتب. |
| [getIconId()](#getIconId--) | يمثل معرّف نوع مجموعة الأيقونات. |
| [getIconSetType()](#getIconSetType--) | يمثل نوع مجموعة الأيقونات. |
| [getIndex()](#getIndex--) | يحصل على فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [getOrder()](#getOrder--) | يشير إلى ترتيب الفرز. |
| [getType()](#getType--) | يمثل نوع الفرز. |
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
### getColor() {#getColor--}
```
public Color getColor()
```


يحصل على اللون المرتب.

**Remarks**

يعمل فقط عندما يكون [getType()](../../com.aspose.cells/datasorterkey\#getType--) هو [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) أو [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


يمثل معرّف نوع مجموعة الأيقونات.

**Remarks**

يعمل فقط عندما يكون [getType()](../../com.aspose.cells/datasorterkey\#getType--) هو [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


يمثل نوع مجموعة الأيقونات.

انظر [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

يعمل فقط عندما يكون [getType()](../../com.aspose.cells/datasorterkey\#getType--) هو [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


يشير إلى ترتيب الفرز.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


يمثل نوع الفرز.

انظر [SortOnType](../../com.aspose.cells/sortontype).

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

