---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعدادات دفتر العمل."
type: docs
url: /ar/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

يمثل إعدادات دفتر العمل.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | يحصل على مؤلف الملف. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | يشير إلى ما إذا كان يتم التحقق من تنسيق الأرقام المخصص عند ضبط Style.Custom، القيمة الافتراضية هي false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | يشير إلى ما إذا كان يتم إنشاء سلسلة الصيغ المحسوبة. |
| [getDate1904()](#getDate1904--) | يحصل على قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904. |
| [getEnableMacros()](#getEnableMacros--) | تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف. |
| [getForceFullCalculate()](#getForceFullCalculate--) | يشير إلى ما إذا كان يتم حساب كامل في كل مرة يتم فيها تشغيل عملية حساب. |
| [getIteration()](#getIteration--) | يشير إلى ما إذا كان يتم استخدام التكرار لحل المراجع الدائرية. |
| [getMaxIteration()](#getMaxIteration--) | إرجاع أو تعيين الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | يشير إلى ما إذا كان سيتم إعادة حساب جميع الصيغ عند فتح الملف. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يضبط مؤلف الملف. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | يشير إلى ما إذا كان يتم التحقق من تنسيق الأرقام المخصص عند ضبط Style.Custom، القيمة الافتراضية هي false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | يشير إلى ما إذا كان يتم إنشاء سلسلة الصيغ المحسوبة. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | يضبط قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | يشير إلى ما إذا كان يتم حساب كامل في كل مرة يتم فيها تشغيل عملية حساب. |
| [setIteration(boolean value)](#setIteration-boolean-) | يشير إلى ما إذا كان يتم استخدام التكرار لحل المراجع الدائرية. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | إرجاع أو تعيين الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | يشير إلى ما إذا كان سيتم إعادة حساب جميع الصيغ عند فتح الملف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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


يشير إلى ما إذا كان يتم التحقق من تنسيق الأرقام المخصص عند ضبط Style.Custom، القيمة الافتراضية هي false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان سيتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة السلسلة التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة لسلاسل النصوص إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق ملف Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُولد. القيمة الافتراضية هي false.

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


يشير إلى ما إذا كان سيتم إنشاء سلسلة الصيغ المحسوبة. القيمة الافتراضية هي false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


يحصل على قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


يشير إلى ما إذا كان يتم حساب كامل في كل مرة يتم فيها تشغيل عملية حساب.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


يشير إلى ما إذا كان يتم استخدام التكرار لحل المراجع الدائرية.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


إرجاع أو تعيين الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما تُعرض.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


يشير إلى ما إذا كان سيتم إعادة حساب جميع الصيغ عند فتح الملف. القيمة الافتراضية هي true.

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


يشير إلى ما إذا كان يتم التحقق من تنسيق الأرقام المخصص عند ضبط Style.Custom، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان سيتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة السلسلة التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة لسلاسل النصوص إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق ملف Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُولد. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


يشير إلى ما إذا كان سيتم إنشاء سلسلة الصيغ المحسوبة. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


يضبط قيمة تمثل ما إذا كان دفتر العمل يستخدم نظام التاريخ 1904.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


يشير إلى ما إذا كان يتم حساب كامل في كل مرة يتم فيها تشغيل عملية حساب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


يشير إلى ما إذا كان يتم استخدام التكرار لحل المراجع الدائرية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


إرجاع أو تعيين الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100.

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

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


يشير إلى ما إذا كان سيتم إعادة حساب جميع الصيغ عند فتح الملف. القيمة الافتراضية هي true.

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

