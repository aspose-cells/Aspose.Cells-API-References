---
title: "NameCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة جميع الكائنات في جدول البيانات."
type: docs
url: /ar/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

يمثل مجموعة جميع كائنات [Name](../../com.aspose.cells/name) في جدول البيانات.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String text)](#add-java.lang.String-) | يحدد اسمًا جديدًا. |
| [clear()](#clear--) | إزالة جميع الأسماء المعرفة التي لا يتم الإشارة إليها في الصيغ ومصدر البيانات. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | الحصول على جميع الأسماء المعرفة حسب النطاق. |
| [get(int index)](#get-int-) | الحصول على عنصر [Name](../../com.aspose.cells/name) عند الفهرس المحدد. |
| [get(String text)](#get-java.lang.String-) | الحصول على عنصر [Name](../../com.aspose.cells/name) بالاسم المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | إزالة الاسم. |
| [remove(String[] names)](#remove-java.lang.String---) | إزالة مصفوفة من الأسماء |
| [removeAt(int index)](#removeAt-int-) | إزالة الاسم عند الفهرس المحدد. |
| [removeDuplicateNames()](#removeDuplicateNames--) | إزالة الأسماء المعرفة المكررة |
| [sort()](#sort--) | فرز الأسماء المعرفة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


يحدد اسمًا جديدًا.

**Remarks**

لا يمكن أن يحتوي الاسم على مسافات ولا يمكن أن يشبه مراجع الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | النص لاستخدامه كاسم. |

**Returns:**
int - فهرس كائن [Name](../../com.aspose.cells/name).
### clear() {#clear--}
```
public void clear()
```


إزالة جميع الأسماء المعرفة التي لا يتم الإشارة إليها في الصيغ ومصدر البيانات. إذا تم الإشارة إلى الاسم المعرفة، فإننا نضبط فقط Name.ReferTo كقيمة فارغة (null) ونخفيها.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


الحصول على جميع الأسماء المعرفة حسب النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). نوع النطاق. |
| sheetIndex | int | فهرس الورقة. يؤثر فقط عندما يكون نوع النطاق هو [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


الحصول على عنصر [Name](../../com.aspose.cells/name) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


الحصول على عنصر [Name](../../com.aspose.cells/name) بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص الاسم. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


إزالة الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص الاسم. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


إزالة مصفوفة من الأسماء

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الأسماء | java.lang.String[] | نص الأسماء. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


إزالة الاسم عند الفهرس المحدد.

**Remarks**

يرجى التأكد من عدم الإشارة إلى الاسم من قبل الصيغ الأخرى قبل استدعاء الطريقة. وإذا تم الإشارة إلى الاسم، فإن تعيين Name.RefersTo إلى null يكون أفضل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الاسم الذي سيتم إزالته. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


إزالة الأسماء المعرفة المكررة

### sort() {#sort--}
```
public void sort()
```


فرز الأسماء المعرفة.

**Remarks**

إذا قمت بإنشاء عدد كبير من النطاقات المسماة في ملف Excel، يرجى استدعاء هذا الأسلوب بعد إنشاء جميع النطاقات المسماة وقبل الحفظ.

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

