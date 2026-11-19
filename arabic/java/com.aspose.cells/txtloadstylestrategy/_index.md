---
title: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد كيفية تطبيق النمط للقيم المُحللة عند تحويل قيمة نصية إلى رقم أو تاريخ/وقت."
type: docs
url: /ar/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

يحدد كيفية تطبيق النمط للقيم المُحللة عند تحويل قيمة نصية إلى رقم أو تاريخ/وقت.
## حقول

| حقل | الوصف |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | عيّن النمط كرقم/تاريخ مدمج عندما تكون القيمة التي تم تحليلها قيمًا رقمية/تاريخية بسيطة. |
| [EXACT_FORMAT](#EXACT-FORMAT) | عيّن التنسيق المخصص الدقيق للقيمة التي تم تحليلها لجعل القيمة المنسقة مطابقة للقيمة الأصلية المدخلة. |
| [NONE](#NONE) | لا يعيّن نمطًا للقيمة التي تم تحليلها. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


عيّن النمط كرقم/تاريخ مدمج عندما تكون القيمة التي تم تحليلها قيمًا رقمية/تاريخية بسيطة.

**Remarks**

عند قيام ms excel بتحليل قيم التاريخ/الوقت أو القيم الرقمية وفقًا لإدخال المستخدم (مثل ملف CSV)، قد يتغير تنسيق تلك القيم، مثل الأصفار المتقدمة/اللاحقة للرقم، ترتيب السنة/الشهر/اليوم للتاريخ/الوقت، ... إلخ. هذا النوع مخصص لمحاكاة سلوك ms excel.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


عيّن التنسيق المخصص الدقيق للقيمة التي تم تحليلها لجعل القيمة المنسقة مطابقة للقيمة الأصلية المدخلة.

### NONE {#NONE}
```
public static final int NONE
```


لا يعيّن نمطًا للقيمة التي تم تحليلها.

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

