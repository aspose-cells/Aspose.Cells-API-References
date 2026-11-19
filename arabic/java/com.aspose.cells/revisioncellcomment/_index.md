---
title: "RevisionCellComment"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل سجل مراجعة لتغيير تعليق الخلية."
type: docs
url: /ar/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

يمثل سجل مراجعة لتغيير تعليق الخلية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | يحصل على نوع الإجراء للمراجعة. |
| [getCellName()](#getCellName--) | يحصل على اسم الخلية. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على فهرس العمود الذي يحتوي على تعليق. |
| [getId()](#getId--) | يحصل على رقم هذا الإصدار. |
| [getNewLength()](#getNewLength--) | يحصل على طول التعليق قبل إجراء هذا التعديل. |
| [getOldLength()](#getOldLength--) | يحصل على طول نص التعليق المضاف في هذا التعديل. |
| [getRow()](#getRow--) | يحصل على فهرس الصف الذي يحتوي على تعليق. |
| [getType()](#getType--) | يحصل على نوع المراجعة. |
| [getWorksheet()](#getWorksheet--) | يحصل على ورقة العمل. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | يشير إلى ما إذا كان تعليقًا قديمًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | يحصل على اسم الخلية. |
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


يحصل على نوع الإجراء للمراجعة.

انظر [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


يحصل على اسم الخلية.

**Returns:**
java.lang.String
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


يحصل على فهرس العمود الذي يحتوي على تعليق.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


يحصل على رقم هذا الإصدار.

**Remarks**

الصفر يعني أن هذا الإصدار لا يحتوي على معرف.

**Returns:**
int
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


يحصل على طول التعليق قبل إجراء هذا التعديل.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


يحصل على طول نص التعليق المضاف في هذا التعديل.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على فهرس الصف الذي يحتوي على تعليق.

**Returns:**
int
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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


يشير إلى ما إذا كان تعليقًا قديمًا.

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




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


يحصل على اسم الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

