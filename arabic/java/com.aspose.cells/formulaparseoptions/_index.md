---
title: "FormulaParseOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الخيارات عند تحليل الصيغة."
type: docs
url: /ar/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

يمثل الخيارات عند تحليل الصيغة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | ما إذا كان يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للدالة المعرفة من قبل المستخدم دون رابط خارجي. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | تعريف لتحليل الدوال المخصصة. |
| [getLocaleDependent()](#getLocaleDependent--) | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |
| [getParse()](#getParse--) | ما إذا كان يتم تحليل الصيغة المعطاة. |
| [getR1C1Style()](#getR1C1Style--) | ما إذا كانت الصيغة بنمط مرجع R1C1. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | ما إذا كان يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للدالة المعرفة من قبل المستخدم دون رابط خارجي. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | تعريف لتحليل الدوال المخصصة. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |
| [setParse(boolean value)](#setParse-boolean-) | ما إذا كان يتم تحليل الصيغة المعطاة. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | ما إذا كانت الصيغة بنمط مرجع R1C1. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


ما إذا كان يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للدالة المعرفة من قبل المستخدم دون رابط خارجي. القيمة الافتراضية هي true (إذا تطابقت الدالة المعرفة من قبل المستخدم مع إحدى الإضافات في الروابط الخارجية الموجودة، فسيتم اعتبارها الإضافة).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


تعريف لتحليل الدوال المخصصة.

**Remarks**

لبعض المتطلبات الخاصة، مثل عند حساب دالة مخصصة في محرك المستخدم المخصص، تحتاج بعض المعلمات إلى حسابها في وضع المصفوفة، يمكن استخدام هذه الخاصية لتحديد تلك المعلمات كالوضع المصفوفي عند تحليل الصيغة. وإلا سيحتاج المستخدم إلى تحديث تلك الدوال المخصصة لاحقًا عبر [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) للحصول على النتيجة نفسها.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. القيمة الافتراضية هي false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


ما إذا كان يتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false، فسيتم الاحتفاظ بسلسلة الصيغة المعطاة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو تُطلب بيانات الصيغة المحللة من قبل عمليات أخرى مثل حساب الصيغ.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


ما إذا كانت الصفة بنمط مرجع R1C1. القيمة الافتراضية هي false.

**Returns:**
boolean
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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


ما إذا كان يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للدالة المعرفة من قبل المستخدم دون رابط خارجي. القيمة الافتراضية هي true (إذا تطابقت الدالة المعرفة من قبل المستخدم مع إحدى الإضافات في الروابط الخارجية الموجودة، فسيتم اعتبارها الإضافة).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


تعريف لتحليل الدوال المخصصة.

**Remarks**

لبعض المتطلبات الخاصة، مثل عند حساب دالة مخصصة في محرك المستخدم المخصص، تحتاج بعض المعلمات إلى حسابها في وضع المصفوفة، يمكن استخدام هذه الخاصية لتحديد تلك المعلمات كالوضع المصفوفي عند تحليل الصيغة. وإلا سيحتاج المستخدم إلى تحديث تلك الدوال المخصصة لاحقًا عبر [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-) للحصول على النتيجة نفسها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


ما إذا كان يتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false، فسيتم الاحتفاظ بسلسلة الصيغة المعطاة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو تُطلب بيانات الصيغة المحللة من قبل عمليات أخرى مثل حساب الصيغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


ما إذا كانت الصفة بنمط مرجع R1C1. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

