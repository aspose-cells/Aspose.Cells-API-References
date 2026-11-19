---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعدادات المصنف."
type: docs
url: /ar/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

يمثل إعدادات دفتر العمل.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | المنشئ الافتراضي |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | يحصل على مؤلف الملف. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | يحصل على ما إذا كان يتم فحص تنسيق الرقم المخصص عند تعيين Style.Custom. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | يحصل على ما إذا كان يتم إنشاء سلسلة الصيغ المحسوبة. |
| [getDate1904()](#getDate1904--) | يحصل على القيمة التي تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904. |
| [getEnableMacros()](#getEnableMacros--) | يحصل على ما إذا كان تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف. |
| [getForceFullCalculate()](#getForceFullCalculate--) | يعيد ما إذا كان يتم الحساب بالكامل في كل مرة يتم فيها تشغيل عملية حسابية. |
| [getIteration()](#getIteration--) | يعيد ما إذا كان يستخدم التكرار لحل الإشارات الدائرية. |
| [getMaxIteration()](#getMaxIteration--) | يعيد الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | يعيد ما إذا كان يعيد حساب جميع الصيغ عند فتح الملف. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يضبط مؤلف الملف. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | يضبط ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | يضبط ما إذا كان يتم إنشاء سلسلة صيغ محسوبة. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | يضبط القيمة التي تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | يضبط ما إذا كان يتم تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | يضبط ما إذا كان يتم الحساب بالكامل في كل مرة يتم فيها تشغيل عملية حسابية. |
| [setIteration(boolean value)](#setIteration-boolean-) | يضبط ما إذا كان يستخدم التكرار لحل الإشارات الدائرية. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | يضبط الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | يضبط ما إذا كان يعيد حساب جميع الصيغ عند فتح الملف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


المنشئ الافتراضي

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


يحصل على مؤلف الملف.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


يحصل على ما إذا كان يتم فحص تنسيق الرقم المخصص عند تعيين Style.Custom.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


يعيد ما إذا كان يتم إنشاء سلسلة صيغ محسوبة. القيمة الافتراضية هي false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


يحصل على القيمة التي تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


يحصل على ما إذا كان تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


يعيد ما إذا كان يتم الحساب بالكامل في كل مرة يتم فيها تشغيل عملية حسابية.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


يعيد ما إذا كان يستخدم التكرار لحل الإشارات الدائرية.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


يعيد الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي تم حشوها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

**Remarks**

عادةً ما تكون تلك المسافات وفواصل الأسطر مجرد غرض بصري، ولا يؤثر الحفاظ عليها أو عدمه على النتيجة المحسوبة. لأسباب تتعلق بالأداء، إذا لم يكن هناك متطلب خاص، فمن الأفضل عدم الحفاظ عليها أثناء معالجة الصيغ.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


يعيد ما إذا كان يعيد حساب جميع الصيغ عند فتح الملف.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


يضبط مؤلف الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


يضبط ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


يضبط ما إذا كان يتم إنشاء سلسلة صيغ محسوبة. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


يضبط القيمة التي تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


يضبط ما إذا كان يتم تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


يضبط ما إذا كان يتم الحساب بالكامل في كل مرة يتم فيها تشغيل عملية حسابية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


يضبط ما إذا كان يستخدم التكرار لحل الإشارات الدائرية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


يضبط الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي تم حشوها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

**Remarks**

عادةً ما تكون تلك المسافات وفواصل الأسطر مجرد غرض بصري، ولا يؤثر الحفاظ عليها أو عدمه على النتيجة المحسوبة. لأسباب تتعلق بالأداء، إذا لم يكن هناك متطلب خاص، فمن الأفضل عدم الحفاظ عليها أثناء معالجة الصيغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


يضبط ما إذا كان يعيد حساب جميع الصيغ عند فتح الملف.

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

