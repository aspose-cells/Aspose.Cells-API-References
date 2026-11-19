---
title: "RevisionCellChange"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل المراجعة التي تغير الخلايا."
type: docs
url: /ar/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

يمثل المراجعة التي تغير الخلايا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | يحصل على اسم الخلية. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على فهرس العمود للخلية. |
| [getId()](#getId--) | يحصل على رقم هذا الإصدار. |
| [getNewFormula()](#getNewFormula--) | يحصل على الصيغة القديمة. |
| [getNewStyle()](#getNewStyle--) | يحصل على النمط الجديد للخلية. |
| [getNewValue()](#getNewValue--) | يحصل على القيمة الجديدة للخلية. |
| [getOldFormula()](#getOldFormula--) | يحصل على الصيغة القديمة. |
| [getOldStyle()](#getOldStyle--) | يحصل على النمط القديم للخلية. |
| [getOldValue()](#getOldValue--) | يحصل على القيمة القديمة للخلية. |
| [getRow()](#getRow--) | يحصل على فهرس الصف للخلية. |
| [getType()](#getType--) | يمثل نوع المراجعة. |
| [getWorksheet()](#getWorksheet--) | يحصل على ورقة العمل. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | يشير إلى ما إذا كانت هذه الخلية مُنسقة حديثًا. |
| [isOldFormatted()](#isOldFormatted--) | يشير إلى ما إذا كانت هذه الخلية مُنسقة قديمًا. |
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


يحصل على فهرس العمود للخلية.

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


يحصل على الصيغة القديمة.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


يحصل على النمط الجديد للخلية.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


يحصل على القيمة الجديدة للخلية.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


يحصل على الصيغة القديمة.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


يحصل على النمط القديم للخلية.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


يحصل على القيمة القديمة للخلية.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على فهرس الصف للخلية.

**Returns:**
int
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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


يشير إلى ما إذا كانت هذه الخلية مُنسقة حديثًا.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


يشير إلى ما إذا كانت هذه الخلية مُنسقة قديمًا.

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

