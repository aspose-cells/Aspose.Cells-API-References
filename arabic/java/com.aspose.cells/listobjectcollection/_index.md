---
title: "ListObjectCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة من الكائنات في ورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/listobjectcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ListObjectCollection extends CollectionBase
```

يمثل مجموعة من الكائنات [ListObject](../../com.aspose.cells/listobject) في ورقة العمل.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#add-int-int-int-int-boolean-) | يضيف ListObject إلى ورقة العمل. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String startCell, String endCell, boolean hasHeaders)](#add-java.lang.String-java.lang.String-boolean-) | يضيف ListObject إلى ورقة العمل. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على ListObject حسب الفهرس. |
| [get(String tableName)](#get-java.lang.String-) | يحصل على ListObject بالاسم المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة [ListObject](../../com.aspose.cells/listobject) حسب الفهرس. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | تحديث جميع أسماء الأعمدة للجداول. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#add-int-int-int-int-boolean-}
```
public int add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


يضيف ListObject إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية لنطاق القائمة. |
| startColumn | int | صف البداية لنطاق القائمة. |
| endRow | int | صف البداية لنطاق القائمة. |
| endColumn | int | صف البداية لنطاق القائمة. |
| hasHeaders | boolean | هل يحتوي النطاق على رؤوس. |

**Returns:**
int - فهرس ListObject الجديد
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### add(String startCell, String endCell, boolean hasHeaders) {#add-java.lang.String-java.lang.String-boolean-}
```
public int add(String startCell, String endCell, boolean hasHeaders)
```


يضيف ListObject إلى ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startCell | java.lang.String | خلية البداية لنطاق القائمة. |
| endCell | java.lang.String | خلية النهاية لنطاق القائمة. |
| hasHeaders | boolean | هل يحتوي النطاق على رؤوس. |

**Returns:**
int - فهرس ListObject الجديد
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الكائنات من مثيل CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
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
### get(int index) {#get-int-}
```
public ListObject get(int index)
```


يحصل على ListObject حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
### get(String tableName) {#get-java.lang.String-}
```
public ListObject get(String tableName)
```


يحصل على ListObject بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tableName | java.lang.String | اسم ListObject. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


إزالة [ListObject](../../com.aspose.cells/listobject) حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


تحديث جميع أسماء الأعمدة للجداول.

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

