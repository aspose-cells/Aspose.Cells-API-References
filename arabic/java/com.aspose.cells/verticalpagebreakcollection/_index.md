---
title: "VerticalPageBreakCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/verticalpagebreakcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VerticalPageBreakCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int column)](#add-int-) | يضيف فاصل صفحة عمودي إلى المجموعة. |
| [add(int row, int column)](#add-int-int-) | يضيف فاصل صفحة عمودي إلى المجموعة. |
| [add(int startRow, int endRow, int column)](#add-int-int-int-) | يضيف فاصل صفحة عمودي إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | يضيف فاصل صفحة عمودي إلى المجموعة. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) عند الفهرس المحدد. |
| [get(String cellName)](#get-java.lang.String-) | يحصل على عنصر [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) بالاسم الخلية المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل عنصر VPageBreak عند اسم محدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int column) {#add-int-}
```
public int add(int column)
```


يضيف فاصل صفحة عمودي إلى المجموعة.

**Remarks**

يتم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس عمود الخلية، يبدأ من الصفر. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) فهرس الكائن.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


يضيف فاصل صفحة عمودي إلى المجموعة.

**Remarks**

يتم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس صف الخلية، يبدأ من الصفر. |
| عمود | int | فهرس عمود الخلية، يبدأ من الصفر. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) فهرس الكائن.
### add(int startRow, int endRow, int column) {#add-int-int-int-}
```
public int add(int startRow, int endRow, int column)
```


يضيف فاصل صفحة عمودي إلى المجموعة.

**Remarks**

يُستخدم هذا الأسلوب لإضافة فاصل صفحة عمودي داخل منطقة الطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس صف البداية، يبدأ من الصفر. |
| endRow | int | فهرس صف النهاية، يبدأ من الصفر. |
| عمود | int | فهرس العمود، يبدأ من الصفر. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) فهرس الكائن.
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


يضيف فاصل صفحة عمودي إلى المجموعة.

**Remarks**

يتم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) فهرس الكائن.
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
public VerticalPageBreak get(int index)
```


يحصل على عنصر [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public VerticalPageBreak get(String cellName)
```


يحصل على عنصر [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) بالاسم الخلية المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element with the specified cell name.
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


يزيل عنصر VPageBreak عند اسم محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس العنصر، يبدأ من الصفر. |

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

