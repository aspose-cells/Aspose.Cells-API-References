---
title: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Java API Reference"
description: "يصف قيم نقاط الاستيفاء في شريط البيانات المتدرج أو مجموعة الأيقونات."
type: docs
url: /ar/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

يصف قيم نقاط الاستيفاء في مقياس تدرجي أو dataBar أو iconSet.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | يحصل على نوع كائن قيمة التنسيق الشرطي هذا. |
| [getValue()](#getValue--) | يحصل على قيمة كائن قيمة التنسيق الشرطي هذا. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | يحصل على علامة أكبر من أو يساوي. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | يضبط علامة أكبر من أو يساوي. |
| [setType(int value)](#setType-int-) | يضبط نوع كائن قيمة التنسيق الشرطي هذا. |
| [setValue(Object value)](#setValue-java.lang.Object-) | يضبط قيمة كائن قيمة التنسيق الشرطي هذا. |
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
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيضبط "Value" تلقائيًا إلى null.

انظر [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامه بالاشتراك مع Type.

**Remarks**

إذا كانت القيمة سلسلة وتبدأ بـ "=", فسيتم معالجتها كصيغة، وإلا سنعالجها كقيمة بسيطة.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


يحصل على علامة أكبر من أو يساوي. يُستخدم فقط لمجموعات الأيقونات، يحدد ما إذا كانت قيمة العتبة تستخدم عامل أكبر من أو يساوي. 'false' تشير إلى استخدام 'أكبر من' بدلاً من 'أكبر من أو يساوي'. القيمة الافتراضية هي true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


يضبط علامة أكبر من أو يساوي. يُستخدم فقط لمجموعات الأيقونات، يحدد ما إذا كانت قيمة العتبة تستخدم عامل أكبر من أو يساوي. 'false' تشير إلى استخدام 'أكبر من' بدلاً من 'أكبر من أو يساوي'. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيضبط "Value" تلقائيًا إلى null.

انظر [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


يضبط قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامه بالاشتراك مع Type.

**Remarks**

إذا كانت القيمة سلسلة وتبدأ بـ "=", فسيتم معالجتها كصيغة، وإلا سنعالجها كقيمة بسيطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

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

