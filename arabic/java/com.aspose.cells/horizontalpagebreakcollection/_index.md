---
title: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int row)](#add-int-) | يضيف فاصل صفحة أفقي إلى المجموعة. |
| [add(int row, int column)](#add-int-int-) | يضيف فاصل صفحة أفقي إلى المجموعة. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | يضيف فاصل صفحة أفقي إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | يضيف فاصل صفحة أفقي إلى المجموعة. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) في الفهرس المحدد. |
| [get(String cellName)](#get-java.lang.String-) | يحصل على عنصر [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) بالاسم الخلية المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل عنصر HPageBreak بالاسم المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


يضيف فاصل صفحة أفقي إلى المجموعة.

**Remarks**

يتم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس صف الخلية، يبدأ من الصفر. |

**Returns:**
int - فهرس كائن [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


يضيف فاصل صفحة أفقي إلى المجموعة.

**Remarks**

يتم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس صف الخلية، يبدأ من الصفر. |
| عمود | int | فهرس عمود الخلية، يبدأ من الصفر. |

**Returns:**
int - فهرس كائن [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


يضيف فاصل صفحة أفقي إلى المجموعة.

**Remarks**

يُستخدم هذا الأسلوب لإضافة فاصل صفحة أفقي داخل منطقة الطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف، يبدأ من الصفر. |
| startColumn | int | فهرس عمود البداية، يبدأ من الصفر. |
| endColumn | int | فهرس عمود النهاية، يبدأ من الصفر. |

**Returns:**
int - فهرس كائن [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
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


يضيف فاصل صفحة أفقي إلى المجموعة.

**Remarks**

يتم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |

**Returns:**
int - فهرس كائن [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
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
public HorizontalPageBreak get(int index)
```


يحصل على عنصر [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


يحصل على عنصر [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) بالاسم الخلية المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


يزيل عنصر HPageBreak بالاسم المحدد.

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

