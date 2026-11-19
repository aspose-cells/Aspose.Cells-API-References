---
title: "GridRow"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل صورة واحدة في جدول بيانات."
type: docs
url: /ar/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

يحتوي على الكائن الذي يمثل صورة واحدة في جدول بيانات.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | يحصل على الخلية. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | احصل على الخلية بواسطة الفهرس المحدد في القائمة. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | يحصل على الخلية الأولى في الصف. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع الصف بوحدة النقاط. |
| [getHidden()](#getHidden--) | يشير إلى ما إذا كان الصف مخفيًا. |
| [getIndex()](#getIndex--) | يحصل على فهرس هذا الصف. |
| [getLastCell()](#getLastCell--) | يحصل على الخلية الأخيرة في الصف. |
| [getLastDataCell()](#getLastDataCell--) | يحصل على الخلية الأخيرة في الصف. |
| [getOutlineLevel()](#getOutlineLevel--) | يحصل على مستوى المخطط. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | يشير إلى ما إذا كان الصف يحتوي على أي بيانات |
| [iterator()](#iterator--) | يحصل على مُعدِّد الخلايا |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | يضبط ارتفاع الصف بوحدة النقاط. |
| [setHidden(boolean value)](#setHidden-boolean-) | يشير إلى ما إذا كان الصف مخفيًا. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | يضبط مستوى المخطط. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


يحصل على الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | مؤشر العمود |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


احصل على الخلية بواسطة الفهرس المحدد في القائمة.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة Row.GetEnumerator() لتكرار جميع الخلايا في هذا الصف. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2015. تقدم Aspose اعتذارها عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الموضع. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


يحصل على الخلية الأولى في الصف.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


يحصل على ارتفاع الصف بوحدة النقاط.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


يشير إلى ما إذا كان الصف مخفيًا.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس هذا الصف.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


يحصل على الخلية الأخيرة في الصف.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


يحصل على الخلية الأخيرة في الصف.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


يحصل على مستوى المخطط.

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


يشير إلى ما إذا كان الصف يحتوي على أي بيانات

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على مُعدِّد الخلايا

**Returns:**
java.util.Iterator - مُعدِّد الخلايا
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


يضبط ارتفاع الصف بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


يشير إلى ما إذا كان الصف مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


يضبط مستوى المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte |  |

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

