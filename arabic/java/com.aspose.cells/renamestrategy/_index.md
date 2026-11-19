---
title: "RenameStrategy"
second_title: "Aspose.Cells for Java API Reference"
description: "خيار الإستراتيجية لأسماء الأعمدة المكررة."
type: docs
url: /ar/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

خيار الإستراتيجية لأسماء الأعمدة المكررة.

**Remarks**

عند معالجة البيانات ذات الرؤوس، تتطلب بعض السيناريوهات عدم تكرار الرؤوس لجميع الأعمدة. على سبيل المثال، عند تصدير البيانات إلى جدول بيانات (datatable) ويتطلب أن يُؤخذ الرأس كاسم عمود في جدول البيانات، تكون القيم المكررة للرأس غير صالحة. في مثل هذه الحالات، يمكن للمستخدم تحديد كيفية التعامل معها عن طريق تحديد هذه الإستراتيجية.
## حقول

| حقل | الوصف |
| --- | --- |
| [DIGIT](#DIGIT) | مسمى برقم. |
| [EXCEPTION](#EXCEPTION) | يرمي استثناء. |
| [LETTER](#LETTER) | مسمى بحرف.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


مسمى برقم. الأسماء المكررة ستصبح ...1، ...2، إلخ.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


يرمي استثناء.

### LETTER {#LETTER}
```
public static final int LETTER
```


مسمى بحرف.. الأسماء المكررة ستصبح ...A، ...B، إلخ.

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

