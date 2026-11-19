---
title: "RevisionCellMove"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل سجل مراجعة على الخلايا التي تم نقلها."
type: docs
url: /ar/java/com.aspose.cells/revisioncellmove/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellMove extends Revision
```

يمثل سجل مراجعة لخلية (خلايا) تم نقلها.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestinationArea()](#getDestinationArea--) | يحصل على منطقة الوجهة. |
| [getId()](#getId--) | يحصل على رقم هذا الإصدار. |
| [getSourceArea()](#getSourceArea--) | يحصل على منطقة المصدر. |
| [getSourceWorksheet()](#getSourceWorksheet--) | يحصل على ورقة العمل المصدر. |
| [getType()](#getType--) | يمثل نوع المراجعة. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDestinationArea() {#getDestinationArea--}
```
public CellArea getDestinationArea()
```


يحصل على منطقة الوجهة.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getId() {#getId--}
```
public int getId()
```


يحصل على رقم هذا الإصدار.

**Remarks**

الصفر يعني أن هذا الإصدار لا يحتوي على معرف.

**Returns:**
int
### getSourceArea() {#getSourceArea--}
```
public CellArea getSourceArea()
```


يحصل على منطقة المصدر.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSourceWorksheet() {#getSourceWorksheet--}
```
public Worksheet getSourceWorksheet()
```


يحصل على ورقة العمل المصدر.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getType() {#getType--}
```
public int getType()
```


يمثل نوع المراجعة.

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

