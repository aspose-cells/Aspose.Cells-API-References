---
title: "TxtSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات الحفظ لتنسيق csv/مفصول بعلامات تبويب/تنسيقات نصية أخرى."
type: docs
url: /ar/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

يمثل خيارات الحفظ لتنسيق csv/مفصول بعلامات تبويب/تنسيقات نصية أخرى.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | ينشئ خيارات حفظ ملف نصي. |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | ينشئ خيارات حفظ ملف نصي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | يشير إلى ما إذا كان يتم دائمًا إضافة '\"' لكل حقل. |
| [getCachedFileFolder()](#getCachedFileFolder--) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز الافتراضي. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [getExportAllSheets()](#getExportAllSheets--) | يشير إلى ما إذا كان يتم تصدير جميع الأوراق إلى ملف النص. |
| [getExportArea()](#getExportArea--) | نطاق الخلايا التي سيتم تصديرها. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | يشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفردة كجزء من قيمة خلية واحدة عندما تكون الدالة [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) صحيحة لها. |
| [getFormatStrategy()](#getFormatStrategy--) | يحصل على استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | يشير إلى ما إذا كان يجب إخراج الفواصل للصفوف الفارغة. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | مزود البيانات لحفظ المصنف في وضع خفيف. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getQuoteType()](#getQuoteType--) | يحصل على طريقة اقتباس القيم في ملف النص المُصدَّر. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSeparator()](#getSeparator--) | يحصل على الفاصل الحرفي لملف النص. |
| [getSeparatorString()](#getSeparatorString--) | يحصل على قيمة نصية كفاصل. |
| [getSortExternalNames()](#getSortExternalNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | يشير إلى ما إذا كان يجب قطع الصفوف والأعمدة الفارغة الأولية كما يفعل برنامج مايكروسوفت إكسل. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | يشير إلى ما إذا كان يجب قطع الخلايا الفارغة المتتالية في صف واحد. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | يشير إلى ما إذا كان يتم دائمًا إضافة '\"' لكل حقل. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | يضبط الترميز الافتراضي. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | يشير إلى ما إذا كان يتم تصدير جميع الأوراق إلى ملف النص. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | نطاق الخلايا التي سيتم تصديرها. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | يشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفردة كجزء من قيمة خلية واحدة عندما تكون الدالة [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) صحيحة لها. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | يضبط استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | يشير إلى ما إذا كان يجب إخراج الفواصل للصفوف الفارغة. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | مزود البيانات لحفظ المصنف في وضع خفيف. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setQuoteType(int value)](#setQuoteType-int-) | يضبط طريقة اقتباس القيم في ملف النص المُصدَّر. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [setSeparator(char value)](#setSeparator-char-) | يضبط الفاصل الحرفي لملف النص. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | يضبط قيمة نصية كفاصل. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | يشير إلى ما إذا كان يجب قطع الصفوف والأعمدة الفارغة الأولية كما يفعل برنامج مايكروسوفت إكسل. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | يشير إلى ما إذا كان يجب قطع الخلايا الفارغة المتتالية في صف واحد. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


ينشئ خيارات حفظ ملف نصي.

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


ينشئ خيارات حفظ ملف نصي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). تنسيق الملف. يجب أن يكون [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV) أو [SaveFormat.TSV](../../com.aspose.cells/saveformat\#TSV)، وإلا سيتم تعيين تنسيق الحفظ تلقائيًا إلى [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV). |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


يشير إلى ما إذا كان يتم دائمًا إضافة '\"' لكل حقل. إذا كان صحيحًا فستُقتبس جميع القيم؛ إذا كان خاطئًا فستُقتبس القيم فقط عند الحاجة (على سبيل المثال، عندما تحتوي القيم على أحرف خاصة مثل '\"' , '\\n' أو حرف الفاصل). القيمة الافتراضية هي false.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية QuoteType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

إذا لم يتم تحديد المجلد، تكون القيمة الافتراضية له هي [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). إذا كانت قيمته الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف ذاكرة مؤقتة عند حفظ دفتر العمل.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


يحصل على الترميز الافتراضي.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Returns:**
boolean
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


يشير إلى ما إذا كان يتم تصدير جميع الأوراق إلى ملف النص. إذا كان خاطئًا، يتم تصدير الورقة النشطة فقط، كما في مايكروسوفت إكسل.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


نطاق الخلايا التي سيتم تصديرها.

**Remarks**

إذا تم تحديد المنطقة المصدرة، فإن [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) لن يكون لها أي تأثير.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


يشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفردة كجزء من قيمة خلية عندما تكون [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) صحيحة لها. القيمة الافتراضية هي false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


يحصل على استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة.

انظر [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


يشير إلى ما إذا كان يجب إخراج الفواصل للصفوف الفارغة. القيمة الافتراضية هي false، لذا بشكل افتراضي سيكون محتوى الصف الفارغ فارغًا.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


مزود البيانات لحفظ المصنف في وضع خفيف.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


يحصل على طريقة اقتباس القيم في ملف النص المُصدَّر.

انظر إلى [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على صيغة حفظ الملف.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


يحصل على الفاصل الحرفي لملف النص.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


يحصل على قيمة نصية كفاصل.

**Returns:**
java.lang.String
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Returns:**
boolean
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


يشير إلى ما إذا كان يجب قص الصفوف والأعمدة الفارغة في البداية كما يفعل ms excel. القيمة الافتراضية هي true.

**Remarks**

نفس القاعدة في ms excel، لن يُعتبر الصف/العمود فارغًا إذا كان لديه نمط مخصص، حتى وإن لم يحتوي على بيانات خلايا. عند الحفظ باستخدام وضع LightCells، لا يؤثر هذا الخيار. يجب على المستخدم التحكم في نطاق الإخراج من خلال تنفيذ [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) أو عن طريق تحديد [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


يشير إلى ما إذا كان يجب قص الخلايا الفارغة المتتالية في صف واحد. القيمة الافتراضية هي false.

**Remarks**

عند الحفظ باستخدام وضع LightCells ولم يتم تحديد [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)، لا يؤثر هذا الخيار وسيتم تمديد الصف إلى آخر خلية يقدمها تنفيذ [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false.

**Remarks**

يؤثر فقط بعد استدعاء الطريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


يحصل على رد النداء للتحذير.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


يشير إلى ما إذا كان يتم دائمًا إضافة '\"' لكل حقل. إذا كان صحيحًا فستُقتبس جميع القيم؛ إذا كان خاطئًا فستُقتبس القيم فقط عند الحاجة (على سبيل المثال، عندما تحتوي القيم على أحرف خاصة مثل '\"' , '\\n' أو حرف الفاصل). القيمة الافتراضية هي false.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية QuoteType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

إذا لم يتم تحديد المجلد، تكون القيمة الافتراضية له هي [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). إذا كانت قيمته الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف ذاكرة مؤقتة عند حفظ دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


يضبط الترميز الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


يشير إلى ما إذا كان يتم تصدير جميع الأوراق إلى ملف النص. إذا كان خاطئًا، يتم تصدير الورقة النشطة فقط، كما في مايكروسوفت إكسل.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


نطاق الخلايا التي سيتم تصديرها.

**Remarks**

إذا تم تحديد المنطقة المصدرة، فإن [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) لن يكون لها أي تأثير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


يشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفردة كجزء من قيمة خلية عندما تكون [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) صحيحة لها. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


يضبط استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة.

انظر [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


يشير إلى ما إذا كان يجب إخراج الفواصل للصفوف الفارغة. القيمة الافتراضية هي false، لذا بشكل افتراضي سيكون محتوى الصف الفارغ فارغًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


مزود البيانات لحفظ المصنف في وضع خفيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


يضبط طريقة اقتباس القيم في ملف النص المُصدَّر.

انظر إلى [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


يضبط الفاصل الحرفي لملف النص.

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

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


يشير إلى ما إذا كان يجب قص الصفوف والأعمدة الفارغة في البداية كما يفعل ms excel. القيمة الافتراضية هي true.

**Remarks**

نفس القاعدة في ms excel، لن يُعتبر الصف/العمود فارغًا إذا كان لديه نمط مخصص، حتى وإن لم يحتوي على بيانات خلايا. عند الحفظ باستخدام وضع LightCells، لا يؤثر هذا الخيار. يجب على المستخدم التحكم في نطاق الإخراج من خلال تنفيذ [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) أو عن طريق تحديد [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


يشير إلى ما إذا كان يجب قص الخلايا الفارغة المتتالية في صف واحد. القيمة الافتراضية هي false.

**Remarks**

عند الحفظ باستخدام وضع LightCells ولم يتم تحديد [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)، لا يؤثر هذا الخيار وسيتم تمديد الصف إلى آخر خلية يقدمها تنفيذ [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false.

**Remarks**

يؤثر فقط بعد استدعاء الطريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


يضبط رد النداء للتحذير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

