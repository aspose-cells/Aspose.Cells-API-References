---
title: "FormulaSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "إعدادات الصيغ والحساب."
type: docs
url: /ar/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

إعدادات الصيغ والحساب.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | يشير إلى ما إذا كان مطلوبًا من التطبيق إجراء حساب كامل عند فتح المصنف. |
| [getCalculateOnSave()](#getCalculateOnSave--) | يشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند، عندما يكون في وضع الحساب اليدوي. |
| [getCalculationId()](#getCalculationId--) | يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف. |
| [getCalculationMode()](#getCalculationMode--) | يحصل على وضع حساب المصنف في MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للمعادلات. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية. |
| [getForceFullCalculation()](#getForceFullCalculation--) | يشير إلى ما إذا كان يحسب جميع المعادلات في كل مرة يتم فيها تشغيل حساب. |
| [getMaxChange()](#getMaxChange--) | الحد الأقصى للتغيير لحل مرجع دائري. |
| [getMaxIteration()](#getMaxIteration--) | الحد الأقصى للتكرارات لحل مرجع دائري. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب المعادلات. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | يشير إلى ما إذا كان يجب الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز المعادلة أثناء الحصول على المعادلات وتعيينها. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | يشير إلى ما إذا كان مطلوبًا من التطبيق إجراء حساب كامل عند فتح المصنف. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | يشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند، عندما يكون في وضع الحساب اليدوي. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | يضبط وضع حساب المصنف في MS Excel. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للمعادلات. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | يشير إلى ما إذا كان يحسب جميع المعادلات في كل مرة يتم فيها تشغيل حساب. |
| [setMaxChange(double value)](#setMaxChange-double-) | الحد الأقصى للتغيير لحل مرجع دائري. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | الحد الأقصى للتكرارات لحل مرجع دائري. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب المعادلات. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | يشير إلى ما إذا كان يجب الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز المعادلة أثناء الحصول على المعادلات وتعيينها. |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


يشير إلى ما إذا كان مطلوبًا من التطبيق إجراء حساب كامل عند فتح المصنف.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات إلى ملف الجدول الناتج بحيث يمكن للتطبيقات الأخرى (مثل MS Excel) التصرف وفقًا لذلك عند تحميل الملف الناتج. لأسباب تتعلق بالأداء في معظم تطبيقات المستخدمين، لا نقوم بحساب أي معادلة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


يشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند، عندما يكون في وضع الحساب اليدوي.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. في حالة مايكروسوفت إكسل، إذا كانت قيمة هذه الخاصية أقل من معرف محرك إعادة الحساب المرتبط بالتطبيق الذي يفتح الملف الناتج، سيعيد التطبيق حساب نتائج جميع الصيغ في هذا المصنف فورًا بعد تحميل الملف. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


يحصل على وضع حساب المصنف في MS Excel.

انظر [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدم، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن الوضع الذي تم تعيينه لهذه الخاصية. إذا كان المستخدم يحتاج إلى حساب الصيغ، يرجى دائمًا استدعاء الطرق على الكائنات المختلفة وفقًا للمتطلبات: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...إلخ.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false.

**Remarks**

عندما يكون هناك الكثير من الصيغ في المصنف ويحتاج المستخدم إلى حسابها بشكل متكرر مع تعديل جزء صغير فقط منها، قد يكون تمكين سلسلة الحساب مفيدًا للأداء. من ناحية أخرى، إذا تم تمكين السلسلة، فإن صيانة نموذج السلسلة تتطلب ذاكرة إضافية، كما أنها تتطلب وقتًا إضافيًا من وحدة المعالجة المركزية لبعض العمليات الأخرى مثل تغيير قيمة الخلية أو الصيغ. بعد تغيير هذه الخاصية من false إلى true، سيتم تحليل وبناء سلسلة الحساب في وقت أول حساب للمصنف، لذا قد يكون الوقت المطلوب لأول حساب أكثر من الحساب العادي بدون السلسلة.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


يشير إلى ما إذا كان يحسب جميع المعادلات في كل مرة يتم فيها تشغيل حساب.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


الحد الأقصى للتغيير لحل مرجع دائري.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


الحد الأقصى للتكرارات لحل مرجع دائري.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب المعادلات.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


يشير إلى ما إذا كان يجب الحفاظ على تلك المسافات وفواصل الأسطر التي يتم حشوها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

**Remarks**

عادةً ما تكون تلك المسافات وفواصل الأسطر مجرد غرض بصري، ولا يؤثر الحفاظ عليها أو عدمه على النتيجة المحسوبة. لأسباب تتعلق بالأداء، إذا لم يكن هناك متطلب خاص، فمن الأفضل عدم الحفاظ عليها أثناء معالجة الصيغ.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


يشير إلى ما إذا كان مطلوبًا من التطبيق إجراء حساب كامل عند فتح المصنف.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات إلى ملف الجدول الناتج بحيث يمكن للتطبيقات الأخرى (مثل MS Excel) التصرف وفقًا لذلك عند تحميل الملف الناتج. لأسباب تتعلق بالأداء في معظم تطبيقات المستخدمين، لا نقوم بحساب أي معادلة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


يشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند، عندما يكون في وضع الحساب اليدوي.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. في حالة مايكروسوفت إكسل، إذا كانت قيمة هذه الخاصية أقل من معرف محرك إعادة الحساب المرتبط بالتطبيق الذي يفتح الملف الناتج، سيعيد التطبيق حساب نتائج جميع الصيغ في هذا المصنف فورًا بعد تحميل الملف. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


يضبط وضع حساب المصنف في MS Excel.

انظر [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدم، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن الوضع الذي تم تعيينه لهذه الخاصية. إذا كان المستخدم يحتاج إلى حساب الصيغ، يرجى دائمًا استدعاء الطرق على الكائنات المختلفة وفقًا للمتطلبات: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...إلخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false.

**Remarks**

عندما يكون هناك الكثير من الصيغ في المصنف ويحتاج المستخدم إلى حسابها بشكل متكرر مع تعديل جزء صغير فقط منها، قد يكون تمكين سلسلة الحساب مفيدًا للأداء. من ناحية أخرى، إذا تم تمكين السلسلة، فإن صيانة نموذج السلسلة تتطلب ذاكرة إضافية، كما أنها تتطلب وقتًا إضافيًا من وحدة المعالجة المركزية لبعض العمليات الأخرى مثل تغيير قيمة الخلية أو الصيغ. بعد تغيير هذه الخاصية من false إلى true، سيتم تحليل وبناء سلسلة الحساب في وقت أول حساب للمصنف، لذا قد يكون الوقت المطلوب لأول حساب أكثر من الحساب العادي بدون السلسلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


يشير إلى ما إذا كان يحسب جميع المعادلات في كل مرة يتم فيها تشغيل حساب.

**Remarks**

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) أن تتصرف وفقًا لذلك عند تحميل الملف ومعالجة الملف الناتج. لأسباب تتعلق بالأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


الحد الأقصى للتغيير لحل مرجع دائري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


الحد الأقصى للتكرارات لحل مرجع دائري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب المعادلات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


يشير إلى ما إذا كان يجب الحفاظ على تلك المسافات وفواصل الأسطر التي يتم حشوها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

**Remarks**

عادةً ما تكون تلك المسافات وفواصل الأسطر مجرد غرض بصري، ولا يؤثر الحفاظ عليها أو عدمه على النتيجة المحسوبة. لأسباب تتعلق بالأداء، إذا لم يكن هناك متطلب خاص، فمن الأفضل عدم الحفاظ عليها أثناء معالجة الصيغ.

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

