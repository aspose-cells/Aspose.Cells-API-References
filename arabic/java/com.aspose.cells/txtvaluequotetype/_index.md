---
title: "TxtValueQuoteType"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد نوع استخدام علامات الاقتباس للقيم في ملفات النص."
type: docs
url: /ar/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

يحدد نوع استخدام علامات الاقتباس للقيم في ملفات النص.
## حقول

| حقل | الوصف |
| --- | --- |
| [ALWAYS](#ALWAYS) | سيتم اقتباس جميع القيم دائمًا. |
| [MINIMUM](#MINIMUM) | اقتبس القيم فقط عند الحاجة. |
| [NEVER](#NEVER) | لن يتم اقتباس جميع القيم. |
| [NORMAL](#NORMAL) | سيتم اقتباس جميع القيم التي تحتوي على أحرف خاصة مثل علامة الاقتباس أو حرف الفاصل. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


سيتم اقتباس جميع القيم دائمًا.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


اقتبس القيم فقط عند الحاجة. على سبيل المثال، إذا كانت قيمة واحدة تحتوي على علامة اقتباس لكن علامة الاقتباس ليست في بداية هذه القيمة، فلن يتم اقتباس هذه القيمة.

### NEVER {#NEVER}
```
public static final int NEVER
```


لن يتم اقتباس جميع القيم. قد لا يتم قراءة ملف النص المُصدَّر بهذا النوع بشكل صحيح لأن علامات الاقتباس المطلوبة غير موجودة.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


جميع القيم التي تحتوي على أحرف خاصة مثل علامة الاقتباس أو حرف الفاصل سيتم اقتباسها. وهذا مشابه لسلوك برنامج مايكروسوفت إكسل عند تصدير ملف نصي.

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

