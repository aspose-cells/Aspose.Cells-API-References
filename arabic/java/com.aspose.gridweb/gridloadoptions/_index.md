---
title: "GridLoadOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات تحميل الملف."
type: docs
url: /ar/java/com.aspose.gridweb/gridloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridLoadOptions
```

يمثل خيارات تحميل الملف. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridLoadOptions()](#GridLoadOptions--) | ينشئ خيارات لتحميل الملف. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [getCheckDataValid()](#getCheckDataValid--) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. |
| [getOnlyAuto()](#getOnlyAuto--) | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. |
| [getPassword()](#getPassword--) | يحصل على كلمة مرور دفتر العمل. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يضبط كلمة مرور المصنف. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridLoadOptions() {#GridLoadOptions--}
```
public GridLoadOptions()
```


ينشئ خيارات لتحميل الملف.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات.

**Remarks**

أحيانًا رغم ضبط الفلتر التلقائي، لا يتم إخفاء الصفوف المقابلة في الملف. الآن يعمل فقط لملف SpreadSheetML.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


تحقق مما إذا كانت البيانات صالحة في ملف القالب.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true ستحصل على استثناء. إذا كانت false، سنقبل قيمة السلسلة التي أدخلتها كقيمة للخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً

**Remarks**

فقط لملف xlsx.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true.

**Remarks**

في السيناريوهات التي يحتاج فيها المستخدم فقط إلى قراءة بعض المحتويات من ملف القالب ولا يحتاج إلى حفظ المصنف مرة أخرى، قد يؤدي ضبط هذه الخاصية إلى false إلى تحسين الأداء، خاصةً عند استخدامها مع نوع من LoadFilter،

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف.

**Remarks**

ينطبق فقط على ملفات Excel Xlsx، Xltx، Xltm و Xlsm لأن الصيغ في الملفات تُخزن كسلسلة نصية.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false.

**Remarks**

ينطبق فقط على ملفات Excel Xlsx، Xltx، Xltm، Xlsm و xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


يحصل على كلمة مرور دفتر العمل.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي تم حشوها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

**Remarks**

بعد تحميل المصنف من ملف القالب باستخدام هذا الخيار، سيتم تعيين [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) إلى نفس القيمة مع هذه الخاصية.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات.

**Remarks**

أحيانًا رغم ضبط الفلتر التلقائي، لا يتم إخفاء الصفوف المقابلة في الملف. الآن يعمل فقط لملف SpreadSheetML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


تحقق مما إذا كانت البيانات صالحة في ملف القالب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true ستحصل على استثناء. إذا كانت false، سنقبل قيمة السلسلة التي أدخلتها كقيمة للخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً

**Remarks**

فقط لملف xlsx.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true.

**Remarks**

في السيناريوهات التي يحتاج فيها المستخدم فقط إلى قراءة بعض المحتويات من ملف القالب ولا يحتاج إلى حفظ المصنف مرة أخرى، قد يؤدي ضبط هذه الخاصية إلى false إلى تحسين الأداء، خاصةً عند استخدامها مع نوع من LoadFilter،

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف.

**Remarks**

ينطبق فقط على ملفات Excel Xlsx، Xltx، Xltm و Xlsm لأن الصيغ في الملفات تُخزن كسلسلة نصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false.

**Remarks**

ينطبق فقط على ملفات Excel Xlsx، Xltx، Xltm، Xlsm و xlsb.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


يضبط كلمة مرور المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي تم حشوها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.

**Remarks**

بعد تحميل المصنف من ملف القالب باستخدام هذا الخيار، سيتم تعيين [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) إلى نفس القيمة مع هذه الخاصية.

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

