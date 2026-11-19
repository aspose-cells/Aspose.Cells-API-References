---
title: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells for Java API Reference"
description: "يسرد استراتيجيات التعامل مع دقة الحساب."
type: docs
url: /ar/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

يسرد استراتيجيات معالجة دقة الحساب. بسبب مشكلة الدقة في حسابات IEEE 754 ذات النقطة العائمة، قد لا يتم حساب بعض الصيغ "البسيطة ظاهريًا" كما هو متوقع. على سبيل المثال الصيغة "=-0.45+0.43+0.02"، عند حساب القيم باستخدام عامل '+' مباشرةً، النتيجة ليست صفرًا. بالنسبة لهذا النوع من مشكلات الدقة، قد توفر بعض الاستراتيجيات الخاصة النتيجة المتوقعة.
## حقول

| حقل | الوصف |
| --- | --- |
| [DECIMAL](#DECIMAL) | يستخدم العشري كمعاملات عندما يكون ذلك ممكنًا. |
| [NONE](#NONE) | لم يتم تطبيق أي استراتيجية على الحساب. |
| [ROUND](#ROUND) | يقوم بتقريب نتيجة الحساب وفقًا للأرقام ذات الدقة. |
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
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


يستخدم القيم العشرية كمعاملات عندما يكون ذلك ممكنًا. وهو الأقل كفاءةً من حيث الأداء.

### NONE {#NONE}
```
public static final int NONE
```


لم يتم تطبيق أي استراتيجية على الحساب. عند الحساب يتم استخدام القيمة المزدوجة الأصلية كمعامل وإرجاع النتيجة مباشرة. هذا هو الأكثر كفاءةً من حيث الأداء وينطبق على معظم الحالات.

### ROUND {#ROUND}
```
public static final int ROUND
```


يقوم بتقريب نتيجة الحساب وفقًا للأرقام ذات الدقة.

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

