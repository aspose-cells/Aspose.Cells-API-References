---
title: "OleObjectCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل كائنات OLE المدمجة."
type: docs
url: /ar/java/com.aspose.cells/oleobjectcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class OleObjectCollection extends CollectionBase
```

يمثل كائنات OLE المدمجة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width, byte[] imageData)](#add-int-int-int-int-byte---) | يضيف OleObject إلى المجموعة. |
| [add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile)](#add-int-int-int-int-byte---java.lang.String-) | يضيف OleObject مرتبط إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | إزالة جميع كائنات OLE المضمنة. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [OleObject](../../com.aspose.cells/oleobject) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width, byte[] imageData) {#add-int-int-int-int-byte---}
```
public int add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```


يضيف OleObject إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| الارتفاع | int | ارتفاع oleObject، بوحدة البكسل. |
| العرض | int | عرض oleObject، بوحدة البكسل. |
| imageData | byte[] | صورة كائن ole كمصفوفة بايت. |

**Returns:**
int - فهرس كائن [OleObject](../../com.aspose.cells/oleobject).
### add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile) {#add-int-int-int-int-byte---java.lang.String-}
```
public int add(int topRow, int leftColumn, int height, int width, byte[] imageData, String linkedFile)
```


يضيف OleObject مرتبط إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| الارتفاع | int | ارتفاع oleObject، بوحدة البكسل. |
| العرض | int | عرض oleObject، بوحدة البكسل. |
| imageData | byte[] | صورة كائن ole كمصفوفة بايت. |
| linkedFile | java.lang.String |  |

**Returns:**
int - فهرس كائن [OleObject](../../com.aspose.cells/oleobject).
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
### clear() {#clear--}
```
public void clear()
```


إزالة جميع كائنات OLE المضمنة.

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
public OleObject get(int index)
```


يحصل على عنصر [OleObject](../../com.aspose.cells/oleobject) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - The element at the specified index.
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


يزيل العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس المحدد. |

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

