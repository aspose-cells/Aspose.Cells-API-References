---
title: "GridTxtLoadOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الخيارات لتحميل ملف نصي."
type: docs
url: /ar/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

يمثل الخيارات لتحميل ملف نصي.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | ينشئ الخيارات لتحميل ملف نصي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [getCheckDataValid()](#getCheckDataValid--) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | يحصل على قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. |
| [getConvertNumericData()](#getConvertNumericData--) | يحصل على قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز الافتراضي. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [getKeepPrecision()](#getKeepPrecision--) | يشير إلى ما إذا كان لا يتم تحليل قيمة السلسلة إذا كان طولها 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. |
| [getOnlyAuto()](#getOnlyAuto--) | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. |
| [getPassword()](#getPassword--) | يحصل على كلمة مرور دفتر العمل. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [getSeparator()](#getSeparator--) | يحصل على فاصل الأحرف لملف النص. |
| [getSeparatorString()](#getSeparatorString--) | يحصل على قيمة نصية كفاصل. |
| [getTextQualifier()](#getTextQualifier--) | يحدد محدد النص لقيم الخلايا. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | ما إذا كان يجب معاملة الفواصل المتتالية كواحدة. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | يشير إلى ما إذا كان يجب أخذ علامة الاقتباس المفردة الأولية كجزء من قيمة خلية واحدة. |
| [hasFormula()](#hasFormula--) | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [hasTextQualifier()](#hasTextQualifier--) | ما إذا كان هناك محدد نص لقيمة الخلية. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | صحيح يعني أن الملف يحتوي على عدة ترميزات. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | يضبط قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات تاريخ. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | يضبط قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات رقمية. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | يضبط الترميز الافتراضي. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | ما إذا كان هناك محدد نص لقيمة الخلية. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | يشير إلى ما إذا كان لا يتم تحليل قيمة السلسلة إذا كان طولها 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | صحيح يعني أن الملف يحتوي على عدة ترميزات. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يضبط كلمة مرور المصنف. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [setSeparator(char value)](#setSeparator-char-) | يضبط فاصل الأحرف لملف النص. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | يضبط قيمة نصية كفاصل. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | يحدد محدد النص لقيم الخلايا. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | ما إذا كان يجب معاملة الفواصل المتتالية كواحدة. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | يشير إلى ما إذا كان يجب أخذ علامة الاقتباس المفردة الأولية كجزء من قيمة خلية واحدة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


ينشئ الخيارات لتحميل ملف نصي.

**Remarks**

نوع ملف التحميل الافتراضي هو CSV.

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


يحصل على قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


يحصل على قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


يحصل على الترميز الافتراضي. ينطبق فقط على ملفات csv.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد المسموح. إذا كانت هذه الخاصية true، سيتم تمديد البيانات الإضافية إلى الورقة التالية خلف الحالية (إذا كانت الورقة الحالية هي الأخيرة، سيتم إضافة ورقة جديدة إلى المصنف الحالي). إذا كانت هذه الخاصية false، سيتم تجاهل البيانات التي تتجاوز الحد. القيمة الافتراضية هي false;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً

**Remarks**

فقط لملف xlsx.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


يشير إلى ما إذا كان لا يتم تحليل قيمة السلسلة إذا كان طولها 15.

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


يحصل على فاصل الأحرف لملف النص.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


يحصل على قيمة نصية كفاصل.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


يحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو '\"'.

**Remarks**

عند ضبط هذه الخاصية، سيصبح [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) true تلقائيًا.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


ما إذا كان يجب معاملة الفواصل المتتالية كواحدة.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


يشير إلى ما إذا كان يجب اعتبار علامة الاقتباس المفردة الأولية جزءًا من قيمة الخلية. القيمة الافتراضية هي true. إذا كانت false، سيتم إزالة علامة الاقتباس المفردة الأولية من قيمة الخلية المقابلة وسيتم ضبط [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) كـ true للخلية.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


صحيح يعني أن الملف يحتوي على عدة ترميزات.

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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات تاريخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات رقمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


يضبط الترميز الافتراضي. ينطبق فقط على ملفات csv.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد المسموح. إذا كانت هذه الخاصية true، سيتم تمديد البيانات الإضافية إلى الورقة التالية خلف الحالية (إذا كانت الورقة الحالية هي الأخيرة، سيتم إضافة ورقة جديدة إلى المصنف الحالي). إذا كانت هذه الخاصية false، سيتم تجاهل البيانات التي تتجاوز الحد. القيمة الافتراضية هي false;

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true.

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

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


يشير إلى ما إذا كان لا يتم تحليل قيمة السلسلة إذا كان طولها 15.

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


صحيح يعني أن الملف يحتوي على عدة ترميزات.

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


يضبط فاصل الأحرف لملف النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


يضبط قيمة نصية كفاصل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


يحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو '\"'.

**Remarks**

عند ضبط هذه الخاصية، سيصبح [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) true تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


ما إذا كان يجب معاملة الفواصل المتتالية كواحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


يشير إلى ما إذا كان يجب اعتبار علامة الاقتباس المفردة الأولية جزءًا من قيمة الخلية. القيمة الافتراضية هي true. إذا كانت false، سيتم إزالة علامة الاقتباس المفردة الأولية من قيمة الخلية المقابلة وسيتم ضبط [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) كـ true للخلية.

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

