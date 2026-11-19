---
title: "RevisionInsertDelete"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل سجل مراجعة لإدراج/حذف صف/عمود."
type: docs
url: /ar/java/com.aspose.cells/revisioninsertdelete/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertDelete extends Revision
```

يمثل سجل مراجعة لإدراج/حذف صف/عمود.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | يسترجع نوع الإجراء لهذا التعديل. |
| [getCellArea()](#getCellArea--) | يسترجع نطاق الإدراج/الحذف. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | يحصل على رقم هذا الإصدار. |
| [getRevisions()](#getRevisions--) | يسترجع قائمة التعديلات بهذه العملية. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


يسترجع نوع الإجراء لهذا التعديل.

انظر [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


يسترجع نطاق الإدراج/الحذف.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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
### getRevisions() {#getRevisions--}
```
public RevisionCollection getRevisions()
```


يسترجع قائمة التعديلات بهذه العملية.

**Returns:**
[RevisionCollection](../../com.aspose.cells/revisioncollection)
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

