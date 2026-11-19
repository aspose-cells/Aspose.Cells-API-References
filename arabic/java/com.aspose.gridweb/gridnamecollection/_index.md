---
title: "GridNameCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

يحتوي على مجموعة من كائنات [GridName](../../com.aspose.gridweb/gridname).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | يعرف اسمًا جديدًا في الورقة المحددة. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | يعرف اسمًا عالميًا جديدًا. |
| [clear()](#clear--) | يزيل جميع الأسماء؛ |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [GridName](../../com.aspose.gridweb/gridname) عند الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | يحصل على مُعدد الصفوف |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | إزالة مصفوفة من الأسماء |
| [removeAt(int index)](#removeAt-int-) | إزالة الاسم عند الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


يعرف اسمًا جديدًا في الورقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس الورقة التي يُطبق فيها الاسم. |
| نص | java.lang.String | نص الاسم. لا يمكن أن يحتوي على اسم ورقة. |
| refersTo | java.lang.String | الصيغة التي يُعرّف الاسم للإشارة إليها. يجب أن تحتوي على اسم ورقة. مثال: 'sheet hello!'A1:B2. |

**Returns:**
int - فهرس كائن الاسم.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


يعرف اسمًا عالميًا جديدًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص الاسم. يمكن أن يحتوي على اسم ورقة. |
| refersTo | java.lang.String | الصيغة التي يُعرّف الاسم للإشارة إليها. يجب أن تحتوي على اسم ورقة. مثال: 'sheet hello!'A1:B2. |

**Returns:**
int - فهرس كائن الاسم.
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الأسماء؛

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
public GridName get(int index)
```


يحصل على عنصر [GridName](../../com.aspose.gridweb/gridname) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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


يحصل على حجم المُعدد

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على مُعدد الصفوف

**Returns:**
java.util.Iterator - مُعدد الصفوف
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

يرجى التأكد من أن الاسم غير مُشار إليه من قبل صيغ أخرى قبل استدعاء الطريقة. وإذا كان الاسم مُشار إليه، يرجى فقط تعيين Name.RefersTo إلى null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

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

