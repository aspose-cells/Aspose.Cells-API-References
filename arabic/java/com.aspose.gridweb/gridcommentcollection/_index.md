---
title: "GridCommentCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridcommentcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridCommentCollection
```

يحتوي على مجموعة من كائنات [GridComment](../../com.aspose.gridweb/gridcomment).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | يضيف تعليقًا إلى المجموعة. |
| [add(String cellName)](#add-java.lang.String-) | يضيف تعليقًا إلى المجموعة. |
| [clear()](#clear--) | يزيل جميع التعليقات؛ |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على العنصر [GridComment](../../com.aspose.gridweb/gridcomment) عند الفهرس المحدد. |
| [get(int row, int column)](#get-int-int-) | يحصل على العنصر [GridComment](../../com.aspose.gridweb/gridcomment) في فهرس الصف المحدد وفهرس العمود المحدد. |
| [get(String cellName)](#get-java.lang.String-) | يحصل على العنصر [GridComment](../../com.aspose.gridweb/gridcomment) في الخلية المحددة. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | يحصل على مُعدد الصفوف |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int row, int column)](#removeAt-int-int-) | يزيل التعليق للخلية المحددة. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | يزيل التعليق للخلية المحددة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


يضيف تعليقًا إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس صف الخلية. |
| عمود | int | فهرس عمود الخلية. |

**Returns:**
int - فهرس كائن [GridComment](../../com.aspose.gridweb/gridcomment).
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


يضيف تعليقًا إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |

**Returns:**
int - فهرس كائن [GridComment](../../com.aspose.gridweb/gridcomment).
### clear() {#clear--}
```
public void clear()
```


يزيل جميع التعليقات؛

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
public GridComment get(int index)
```


يحصل على العنصر [GridComment](../../com.aspose.gridweb/gridcomment) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public GridComment get(int row, int column)
```


يحصل على العنصر [GridComment](../../com.aspose.gridweb/gridcomment) في فهرس الصف المحدد وفهرس العمود المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public GridComment get(String cellName)
```


يحصل على العنصر [GridComment](../../com.aspose.gridweb/gridcomment) في الخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
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




### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


يزيل التعليق للخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | فهرس العمود. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


يزيل التعليق للخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية التي تحتوي على تعليق. |

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

