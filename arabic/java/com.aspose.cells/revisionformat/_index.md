---
title: "RevisionFormat"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل سجل مراجعة لمعلومات حول تغيير التنسيق."
type: docs
url: /ar/java/com.aspose.cells/revisionformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionFormat extends Revision
```

يمثل سجل مراجعة لمعلومات حول تغيير التنسيق.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | النطاق الذي تم تطبيق هذا التنسيق عليه. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | يحصل على رقم هذا الإصدار. |
| [getStyle()](#getStyle--) | يحصل على النمط المطبق. |
| [getType()](#getType--) | يحصل على نوع المراجعة. |
| [getWorksheet()](#getWorksheet--) | يحصل على ورقة العمل. |
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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


النطاق الذي تم تطبيق هذا التنسيق عليه.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


يحصل على رقم هذا الإصدار.

**Remarks**

الصفر يعني أن هذا الإصدار لا يحتوي على معرف.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


يحصل على النمط المطبق.

**Returns:**
[Style](../../com.aspose.cells/style)
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع المراجعة.

انظر [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على ورقة العمل.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

