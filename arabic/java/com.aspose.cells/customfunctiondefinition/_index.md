---
title: "CustomFunctionDefinition"
second_title: "Aspose.Cells for Java API Reference"
description: "تعريف الدالة المخصصة للحساب باستخدام محرك المستخدم المخصص."
type: docs
url: /ar/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

تعريف الدالة المخصصة للحساب باستخدام محرك المستخدم المخصص.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | يحصل على مؤشرات معلمات الدالة المخصصة المحددة التي تحتاج إلى حسابها في وضع المصفوفة. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


يحصل على مؤشرات معلمات الدالة المخصصة المحددة التي تحتاج إلى حسابها في وضع المصفوفة.

**Remarks**

لتعبير يحتاج إلى حساب، مع أخذ A:A+B:B كمثال: عادةً في وضع القيمة يتم حسابه إلى قيمة واحدة وفقًا لخلية الأساس الحالية. ولكن في وضع المصفوفة، سيتم حساب جميع القيم A1+B1، A2+B2، A3+B3، ... واستخدامها في الحساب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| functionName | java.lang.String | اسم الدالة المخصصة. |

**Returns:**
int[] - مؤشرات المعلمات التي تحتاج إلى حسابها في وضع المصفوفة للدالة المخصصة المحددة. القيمة الافتراضية هي null، لا توجد معلمة تحتاج إلى حسابها في وضع المصفوفة للدالة المخصصة.
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

