---
title: "SplitPartInfo"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل معلومات إدخال/إخراج واحد لعدة إدخالات/إخراجات مثل الصفحة الحالية التي سيتم عرضها عند تحويل الجدول إلى صورة."
type: docs
url: /ar/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

يمثل معلومات إدخال/إخراج واحد لعدة إدخالات/إخراجات، مثل الصفحة الحالية التي سيتم عرضها عند تحويل جدول البيانات إلى صورة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | فهرس الجزء الحالي في التسلسل (بدءًا من 0) |
| [getSheetIndex()](#getSheetIndex--) | فهرس الورقة التي يوجد فيها الجزء الحالي. -1 يعني وجود ورقة واحدة فقط. |
| [getSheetName()](#getSheetName--) | اسم الورقة التي يوجد فيها الجزء الحالي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


فهرس الجزء الحالي في التسلسل (بدءًا من 0). -1 يعني عدم وجود أجزاء متعددة وبالتالي النتيجة واحدة.

**Remarks**

إذا كان هناك حاجة لمعالجة عدة أوراق وكان كل ورقة تُعالج (تقسيم) بشكل منفصل، فإن فهرس الجزء يبدأ دائمًا من 0 لكل ورقة. على سبيل المثال، عند تحويل دفتر العمل إلى صور، يمثل فهرس صفحة الإخراج للورقة التي تتم معالجتها حاليًا. ويشير -1 إلى وجود صفحة واحدة فقط للورقة الحالية.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


فهرس الورقة التي يوجد فيها الجزء الحالي. -1 يعني وجود ورقة واحدة فقط.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


اسم الورقة التي يوجد فيها الجزء الحالي.

**Remarks**

قد يكون فارغًا في بعض الحالات، مثل عند تحويل دفتر العمل بالكامل إلى صورة TIFF.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

