---
title: "GridCacheForStream"
second_title: "Aspose.Cells for Java API Reference"
description: "تحتوي هذه الفئة على عمليات التخزين المؤقت لـ GridJs."
type: docs
url: /ar/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

هذه الفئة تحتوي على عمليات الذاكرة المؤقتة لـ GridJs. يجب على المستخدم تنفيذ منطق الأعمال الخاص به للتخزين بناءً عليها..
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | تنفذ هذه الطريقة للحصول على عنوان URL للملف من الذاكرة المؤقتة. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | يتحقق مما إذا كانت الذاكرة المؤقتة بالمعرف uid موجودة |
| [loadStream(String uid)](#loadStream-java.lang.String-) | تنفذ هذه الطريقة لتحميل الذاكرة المؤقتة باستخدام المفتاح uid، وتعيد الدفق من الذاكرة المؤقتة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | تنفذ هذه الطريقة لحفظ الذاكرة المؤقتة، وتخزن الدفق في الذاكرة المؤقتة باستخدام المفتاح uid. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```


تنفذ هذه الطريقة للحصول على عنوان URL للملف من الذاكرة المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
java.lang.String - عنوان URL للملف
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```


يتحقق مما إذا كانت الذاكرة المؤقتة بالمعرف uid موجودة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String | المعرف الفريد لذاكرة التخزين المؤقت للملف. |

**Returns:**
boolean - القيمة المنطقية
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


تنفذ هذه الطريقة لتحميل الذاكرة المؤقتة باستخدام المفتاح uid، وتعيد الدفق من الذاكرة المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```


تنفذ هذه الطريقة لحفظ الذاكرة المؤقتة، وتخزن الدفق في الذاكرة المؤقتة باستخدام المفتاح uid.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |

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

