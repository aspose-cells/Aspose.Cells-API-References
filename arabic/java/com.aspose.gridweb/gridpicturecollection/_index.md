---
title: "GridPictureCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridpicturecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPictureCollection
```

يحتوي على مجموعة من كائنات [GridPicture](../../com.aspose.gridweb/gridpicture) objects.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | يضيف صورة إلى المجموعة. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName)](#add-int-int-java.lang.String-) | يضيف صورة إلى المجموعة. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | يضيف صورة إلى المجموعة. |
| [clear()](#clear--) | مسح جميع الصور. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [GridPicture](../../com.aspose.gridweb/gridpicture) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | يحصل على مُعدد الصفوف |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int param_int)](#removeAt-int-) | إزالة الأشكال في الفهرس المحدد |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | int | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | int | فهرس العمود العلوي الأيسر. |
| lowerRightRow | int | فهرس الصف السفلي الأيمن. |
| lowerRightColumn | int | فهرس العمود السفلي الأيمن. |
| fileName | java.lang.String | اسم ملف الصورة. |

**Returns:**
int - فهرس كائن [GridPicture](../../com.aspose.gridweb/gridpicture).
### add(int upperLeftRow, int upperLeftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | int | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | int | فهرس العمود العلوي الأيسر. |
| fileName | java.lang.String | اسم ملف الصورة. |

**Returns:**
int - فهرس كائن [GridPicture](../../com.aspose.gridweb/gridpicture).
### add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | int | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | int | فهرس العمود العلوي الأيسر. |
| fileName | java.lang.String | اسم ملف الصورة. |
| widthScale | int | مقياس عرض الصورة، كنسبة مئوية. |
| heightScale | int | مقياس ارتفاع الصورة، كنسبة مئوية. |

**Returns:**
int - فهرس كائن [GridPicture](../../com.aspose.gridweb/gridpicture).
### clear() {#clear--}
```
public void clear()
```


مسح جميع الصور.

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
public GridPicture get(int index)
```


يحصل على عنصر [GridPicture](../../com.aspose.gridweb/gridpicture) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridPicture](../../com.aspose.gridweb/gridpicture) - The element at the specified index.
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




### removeAt(int param_int) {#removeAt-int-}
```
public void removeAt(int param_int)
```


إزالة الأشكال في الفهرس المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| param_int | int |  |

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

