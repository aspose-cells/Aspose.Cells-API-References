---
title: "RowColumnEventArgs"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر البيانات لأحداث الصف/العمود."
type: docs
url: /ar/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

يوفر البيانات لأحداث الصف/العمود.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | معامل الحدث. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | رقم الصف أو العمود، يبدأ من الصفر. |
| [getType()](#getType--) | نوع الصف أو العمود. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | هل نلغي العملية. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | استدعِ هذه الطريقة في معالجات حدث RowDeleting/ColumnDeleting لإلغاء عمليات الحذف. |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```


معامل الحدث.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


رقم الصف أو العمود، يبدأ من الصفر.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


نوع الصف أو العمود.

انظر [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


هل نلغي العملية.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


استدعِ هذه الطريقة في معالجات حدث RowDeleting/ColumnDeleting لإلغاء عمليات الحذف.

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

