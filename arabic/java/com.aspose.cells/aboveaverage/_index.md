---
title: "AboveAverage"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف قاعدة التنسيق الشرطي AboveAverage."
type: docs
url: /ar/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

صف قاعدة تنسيق الخلايا الشرطي AboveAverage. تُبرز هذه القاعدة الخلايا التي تكون أعلى أو أقل من المتوسط لجميع القيم في النطاق.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | يحصل على عدد الانحرافات المعيارية لتضمينها فوق أو تحت المتوسط في قاعدة تنسيق الخلايا الشرطي. |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | يحصل على العلامة التي تشير إلى ما إذا كانت القاعدة قاعدة "above average". |
| [isEqualAverage()](#isEqualAverage--) | يحصل على العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم تستثنيه. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | يضبط العلامة التي تشير إلى ما إذا كانت القاعدة قاعدة "above average". |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | يضبط العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم تستثنيه. |
| [setStdDev(int value)](#setStdDev-int-) | يضبط عدد الانحرافات المعيارية التي يتم تضمينها فوق أو تحت المتوسط في قاعدة التنسيق الشرطي. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
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
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


يحصل على عدد الانحرافات المعيارية التي يتم تضمينها فوق أو تحت المتوسط في قاعدة التنسيق الشرطي. يجب أن تكون القيمة المدخلة بين 0 و 3 (تشمل 0 و 3). ضبط هذه القيمة إلى 0 يعني أن stdDev غير محدد. القيمة الافتراضية هي 0.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


يحصل على العلامة التي تشير إلى ما إذا كانت القاعدة هي قاعدة "أعلى من المتوسط". 'true' يعني 'أعلى من المتوسط'. القيمة الافتراضية هي true.

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


يحصل على العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم تستثنيه. 'true' يعني تضمين قيمة المتوسط في المعايير. القيمة الافتراضية هي false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


يضبط العلامة التي تشير إلى ما إذا كانت القاعدة هي قاعدة "أعلى من المتوسط". 'true' يعني 'أعلى من المتوسط'. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


يضبط العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم تستثنيه. 'true' يعني تضمين قيمة المتوسط في المعايير. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


يضبط عدد الانحرافات المعيارية التي يتم تضمينها فوق أو تحت المتوسط في قاعدة التنسيق الشرطي. يجب أن تكون القيمة المدخلة بين 0 و 3 (تشمل 0 و 3). ضبط هذه القيمة إلى 0 يعني أن stdDev غير محدد. القيمة الافتراضية هي 0.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

