---
title: "SignificantDigitsType"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل نوع الأرقام ذات الدقة لإخراج القيم الرقمية."
type: docs
url: /ar/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

يمثل نوع الأرقام ذات الدقة لإخراج القيم الرقمية.
## حقول

| حقل | الوصف |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15-أرقام |
| [G_17](#G-17) | 17-أرقام عن طريق تنسيق القيمة باستخدام "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17-أرقام عن طريق تقريب القيمة. |
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
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15-أرقام

### G_17 {#G-17}
```
public static final int G_17
```


17-أرقام عن طريق تنسيق القيمة باستخدام "G17".

**Remarks**

قد تُعطي بعض قيم double، "G17" قيمة مختلفة عن القيمة الأصلية/الحرفية التي أدخلها المستخدم. على سبيل المثال، قيمة double 0.15 ستُخرج كـ 0.14999999999999999؛ قيمة double 1.0E-16 ستُخرج كـ 9.9999999999999998E-17. يتعامل برنامج Ms Excel مع هذه القيم بشكل غير متسق، فهو يحفظ 0.15 كـ 0.15 في ملف xlsx، لكن بالنسبة لـ 1.0E-16 القيمة المحفوظة في ملف xlsx هي 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17-أرقام عن طريق تقريب القيمة.

**Remarks**

هذا النوع عادةً ما يُخرج القيمة كما هي الأصلية/الحرفية التي أدخلها المستخدم. بالنسبة إلى 0.15 ينتج "0.15" ولـ 1.0E-16 ينتج "1.0E-16". ولكن هناك بعض الحالات الخاصة التي قد تعطي قيمًا مختلفة عن الحرفية. على سبيل المثال، عند تقريب 208435494.96478021 إلى 17-أرقام("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#"), يكون الناتج 208435494.96478.

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

