---
title: "SheetSet"
second_title: "Aspose.Cells for Java API Reference"
description: "يصف مجموعة من الأوراق."
type: docs
url: /ar/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

يصف مجموعة من الأوراق.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | ينشئ مجموعة أوراق بناءً على فهارس الأوراق الدقيقة. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | ينشئ مجموعة أوراق بناءً على أسماء الأوراق الدقيقة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | يحصل على مجموعة تحتوي على الورقة النشطة في دفتر العمل. |
| [getAll()](#getAll--) | يحصل على مجموعة تحتوي على جميع أوراق دفتر العمل بترتيبها الأصلي. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | يحصل على مجموعة تحتوي على الأوراق الظاهرة في دفتر العمل بترتيبها الأصلي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


ينشئ مجموعة أوراق بناءً على فهارس الأوراق الدقيقة.

**Remarks**

إذا تم العثور على ورقة غير موجودة في دفتر العمل، سيتم إلقاء استثناء أثناء العرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndexes | int[] | فهارس الأوراق ذات أساس صفر. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


ينشئ مجموعة أوراق بناءً على أسماء الأوراق الدقيقة.

**Remarks**

إذا تم العثور على ورقة غير موجودة في دفتر العمل، سيتم إلقاء استثناء أثناء العرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetNames | java.lang.String[] | أسماء الأوراق. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


يحصل على مجموعة تحتوي على الورقة النشطة في دفتر العمل.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


يحصل على مجموعة تحتوي على جميع أوراق دفتر العمل بترتيبها الأصلي.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


يحصل على مجموعة تحتوي على الأوراق الظاهرة في دفتر العمل بترتيبها الأصلي.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

