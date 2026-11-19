---
title: "PivotPageFields"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عناصر صفحة المحور إذا كان مصدر بيانات جدول المحور هو نطاقات التجميع."
type: docs
url: /ar/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

يمثل عناصر صفحة المحور إذا كان مصدر بيانات جدول المحور هو نطاقات التجميع. يمكن أن يحتوي على ما لا يزيد عن 4 عناصر.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | يمثل عناصر حقل صفحة المحور. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | يحدد أي تسمية عنصر في كل حقل صفحة تُستخدم لتحديد نطاق البيانات. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | يضيف حقل صفحة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | يحصل على عدد حقول الصفحة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


يمثل عناصر حقل صفحة المحور.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


يحدد أي تسمية عنصر في كل حقل صفحة تُستخدم لتحديد نطاق البيانات. يجب أن يكون طول pageItemIndex مساويًا لعدد PageFieldCount، لذا يرجى إضافة حقل الصفحة أولاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rangeIndex | int | فهرس نطاق بيانات التجميع. |
| pageItemIndex | int[] | فهرس عنصر الصفحة في كل حقل صفحة. pageItemIndex[2] = 1 يعني العنصر الثاني في الحقل الثالث يُستخدم لتحديد هذا النطاق. pageItemIndex[1] = -1 يعني لا يوجد عنصر في الحقل الثاني يُستخدم لتحديد هذا النطاق وستقوم MS بإنشاء عنصر \"blank\" تلقائيًا في الحقل الثاني لتحديد هذا النطاق. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


يضيف حقل صفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageItems | java.lang.String[] | تسمية عنصر حقل الصفحة |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


يحصل على عدد حقول الصفحة.

**Returns:**
int
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

