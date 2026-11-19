---
title: "ExternalLinkCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة الروابط الخارجية في مصنف."
type: docs
url: /ar/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

يمثل مجموعة الروابط الخارجية في مصنف.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | أضف رابطًا خارجيًا . |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | يضيف رابطًا خارجيًا. |
| [clear()](#clear--) | يزيل جميع الروابط الخارجية. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | يزيل جميع الروابط الخارجية. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على العنصر [ExternalLink](../../com.aspose.cells/externallink) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة فعليًا في المجموعة. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | احصل على مُعدِّد يتكرر عبر هذه المجموعة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل الرابط الخارجي المحدد من دفتر العمل. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | يزيل الرابط الخارجي المحدد من دفتر العمل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


أضف رابطًا خارجيًا .

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). نوع الدليل لاسم الملف. |
| fileName | java.lang.String | اسم الملف. |
| sheetNames | java.lang.String[] | جميع أسماء الأوراق في الملف الخارجي. |

**Returns:**
int - موضع الاسم الخارجي في هذه القائمة.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


يضيف رابطًا خارجيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف الخارجي. |
| sheetNames | java.lang.String[] | جميع أسماء الأوراق في الملف الخارجي. |

**Returns:**
int - موضع الاسم الخارجي في هذه القائمة.
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الروابط الخارجية.

**Remarks**

عند إزالة الروابط الخارجية، سيتم إزالة جميع الصيغ التي تشير إليها أيضًا لأن المراجع تصبح غير صالحة.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


يزيل جميع الروابط الخارجية.

**Remarks**

إذا كان من الضروري تحديث المراجع، فسيتم تغيير تلك المراجع للروابط الخارجية في الصيغ إلى المصنف الحالي عندما يكون ذلك ممكنًا. على سبيل المثال، الصيغة الأصلية لخلية ما هي "='externalsource.xlam'!customfunction()"، بعد إزالة الروابط الخارجية، ستصبح الصيغة "=customfunction()"؛ عندما تكون الصيغة الأصلية "='[externalsource.xlam]Sheet1'!$A$1"، حسب ما إذا كان هناك ورقة واحدة باسم "Sheet1" في المصنف الحالي: إذا كان الأمر صحيحًا، ستصبح الصيغة "=Sheet1!$A$1"؛ إذا كان خاطئًا، ستصبح الصيغة "=\#REF!$A$1".

إذا لم يكن من الضروري تحديث المراجع، سيتم إزالة جميع الصيغ التي تحتوي على مراجع للروابط الخارجية أيضًا لأن تلك المراجع تصبح غير صالحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | ما إذا كان سيتم تحديث جميع مراجع الروابط الخارجية في الصيغ إلى مراجع المصنف الحالي نفسه. |

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
public ExternalLink get(int index)
```


يحصل على العنصر [ExternalLink](../../com.aspose.cells/externallink) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
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


يحصل على عدد العناصر الموجودة فعليًا في المجموعة.

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


احصل على مُعدِّد يتكرر عبر هذه المجموعة.

**Returns:**
java.util.Iterator -
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


يزيل الرابط الخارجي المحدد من دفتر العمل.

**Remarks**

عند إزالة الرابط الخارجي، سيتم إزالة جميع الصيغ التي تشير إليه أيضًا لأن المراجع تصبح غير صالحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الرابط الخارجي الذي سيتم إزالته. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


يزيل الرابط الخارجي المحدد من دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الرابط الخارجي الذي سيتم إزالته. |
| updateReferencesAsLocal | boolean | ما إذا كان سيتم تحديث جميع مراجع الرابط الخارجي المحدد إلى مرجع المصنف الحالي نفسه. تحقق من [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) للحصول على مزيد من التفاصيل حول هذه المعلمة. |

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

