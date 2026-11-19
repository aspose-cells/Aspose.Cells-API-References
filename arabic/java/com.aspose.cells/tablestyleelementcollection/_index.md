---
title: "TableStyleElementCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع عناصر نمط الجدول."
type: docs
url: /ar/java/com.aspose.cells/tablestyleelementcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleElementCollection extends CollectionBase
```

يمثل جميع عناصر نمط الجدول.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int type)](#add-int-) | يضيف عنصرًا. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر من نمط الجدول حسب الفهرس. |
| [getByTableStyleElementType(int type)](#getByTableStyleElementType-int-) | يحصل على عنصر نمط الجدول حسب نوع العنصر. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getTableStyleElementWithIndex(int index)](#getTableStyleElementWithIndex-int-) | يحصل على عنصر من نمط الجدول حسب الفهرس. |
| [getTableStyleElementWithType(int type)](#getTableStyleElementWithType-int-) | يحصل على عنصر نمط الجدول حسب نوع العنصر. |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


يضيف عنصرًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). نوع العنصر |

**Returns:**
int - يُرجع فهرس العنصر في القائمة.
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
public TableStyleElement get(int index)
```


يحصل على عنصر من نمط الجدول حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
### getByTableStyleElementType(int type) {#getByTableStyleElementType-int-}
```
public TableStyleElement getByTableStyleElementType(int type)
```


يحصل على عنصر نمط الجدول حسب نوع العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). نوع العنصر. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
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
### getTableStyleElementWithIndex(int index) {#getTableStyleElementWithIndex-int-}
```
public TableStyleElement getTableStyleElementWithIndex(int index)
```


يحصل على عنصر من نمط الجدول حسب الفهرس.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية Aspose.Cells.Tables.TableStyleElementCollection.this[int index]. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
### getTableStyleElementWithType(int type) {#getTableStyleElementWithType-int-}
```
public TableStyleElement getTableStyleElementWithType(int type)
```


يحصل على عنصر نمط الجدول حسب نوع العنصر.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية Aspose.Cells.Tables.TableStyleElementCollection.this[TableStyleElementType type]. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| النوع | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
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
| الفهرس | int | الفهرس الصفري للعنصر المراد إزالته. |

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

