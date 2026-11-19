---
title: "AbstractTextLoadOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات شائعة لتحميل قيم النص"
type: docs
url: /ar/java/com.aspose.cells/abstracttextloadoptions/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class AbstractTextLoadOptions extends LoadOptions
```

خيارات شائعة لتحميل قيم النص
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | يحصل على خيارات الضبط التلقائي |
| [getCheckDataValid()](#getCheckDataValid--) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | يحصل على قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. |
| [getConvertNumericData()](#getConvertNumericData--) | يحصل على قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط دفتر العمل |
| [getEncoding()](#getEncoding--) | يحصل على الترميز الافتراضي. |
| [getFontConfigs()](#getFontConfigs--) | يحصل على إعدادات الخط الفردية. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة. |
| [getInterruptMonitor()](#getInterruptMonitor--) | يحصل على مراقب المقاطعة. |
| [getKeepPrecision()](#getKeepPrecision--) | يشير إلى ما إذا كان لا يتم تحليل قيمة السلسلة إذا كان طولها 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. |
| [getLanguageCode()](#getLanguageCode--) | يحصل على لغة واجهة المستخدم لإصدار دفتر العمل بناءً على رمز البلد الذي تم حفظ الملف به. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب. |
| [getLoadFilter()](#getLoadFilter--) | المرشح لتحديد كيفية تحميل البيانات. |
| [getLoadFormat()](#getLoadFormat--) | يحصل على تنسيق التحميل. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | يشير إلى الاستراتيجية لتطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ/وقت. |
| [getLocale()](#getLocale--) | يحصل على الإعدادات الإقليمية المستخدمة لدفتر العمل الذي سيتم تحميله. |
| [getMemorySetting()](#getMemorySetting--) | يحصل على وضع الذاكرة لدفتر العمل المحمَّل. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. |
| [getPassword()](#getPassword--) | يحصل على كلمة مرور دفتر العمل. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [getRegion()](#getRegion--) | يحصل على الإعدادات الإقليمية المستخدمة لدفتر العمل الذي سيتم تحميله. |
| [getStandardFont()](#getStandardFont--) | يضبط اسم الخط القياسي الافتراضي |
| [getStandardFontSize()](#getStandardFontSize--) | يضبط حجم الخط القياسي الافتراضي. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | يضبط خيارات الضبط التلقائي |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | يضبط قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات تاريخ. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | يضبط قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات رقمية. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | يضبط الترميز الافتراضي. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | يضبط إعدادات الخط الفردية. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | يضبط مراقب المقاطعة. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | يشير إلى ما إذا كان لا يتم تحليل قيمة السلسلة إذا كان طولها 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | المرشح لتحديد كيفية تحميل البيانات. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | يشير إلى الاستراتيجية لتطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ/وقت. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | يضبط وضع الذاكرة للمصنف المحمّل. |
| [setPaperSize(int type)](#setPaperSize-int-) | يضبط حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يضبط كلمة مرور المصنف. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. |
| [setRegion(int value)](#setRegion-int-) | يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | يضبط اسم الخط القياسي الافتراضي |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | يضبط حجم الخط القياسي الافتراضي. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات.

**Remarks**

أحيانًا رغم ضبط الفلتر التلقائي، لا يتم إخفاء الصفوف المقابلة في الملف. الآن يعمل فقط لملف SpreadSheetML.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


يحصل على خيارات الضبط التلقائي

**Remarks**

فقط لملف xlsx، spreadsheetML الآن.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
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


يحصل على قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات تاريخ. القيمة الافتراضية هي true.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


يحصل على قيمة تشير إلى ما إذا كانت السلسلة في ملف النص تُحول إلى بيانات رقمية. القيمة الافتراضية هي true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


يحصل على إعدادات النمط الافتراضية لتهيئة أنماط دفتر العمل

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


يحصل على الترميز الافتراضي. ينطبق فقط على ملفات csv.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


يحصل على إعدادات الخط الفردية. يعمل فقط مع الـ [Workbook](../../com.aspose.cells/workbook) الذي يستخدم هذه الـ [LoadOptions](../../com.aspose.cells/loadoptions) للتحميل.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً

**Remarks**

فقط لملف xlsx.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة.

**Remarks**

يعمل فقط لملفات xlsx، xlsb، و xlsm. هناك العديد من الأشكال المتداخلة المتطابقة التي لا فائدة منها في بعض الملفات، يمكننا تجاهلها عند تحميل الملفات.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


يحصل على مراقب المقاطعة.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
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
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


يحصل على لغة واجهة المستخدم لإصدار دفتر العمل بناءً على رمز البلد الذي تم حفظ الملف به.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


المرشح لتحديد كيفية تحميل البيانات.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


يحصل على تنسيق التحميل.

انظر [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


يشير إلى الاستراتيجية لتطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ/وقت.

انظر [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


يحصل على الإعدادات الإقليمية المستخدمة لدفتر العمل الذي سيتم تحميله.

**Remarks**

هذه الخاصية لها نفس التأثير مع [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) لتعيين الإعدادات الإقليمية.

**Returns:**
java.util.Locale
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


يحصل على وضع الذاكرة لدفتر العمل المحمَّل.

انظر [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

لمزيد من التفاصيل حول وضع الذاكرة، يرجى الاطلاع على [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
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

بعد تحميل المصنف من ملف القالب باستخدام هذا الخيار، سيتم تعيين [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) إلى نفس القيمة مع هذه الخاصية.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


يحصل على الإعدادات الإقليمية المستخدمة لدفتر العمل الذي سيتم تحميله.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

قد تُستخدم الإعدادات الإقليمية لتهيئة بعض الميزات للمصنف مثل الخطوط والسمات وما إلى ذلك. بالنسبة لتنسيقات الملفات القائمة على النص، مثل CSV وHTML، ...، سيتم أيضًا استخدام الإعداد الإقليمي لاكتشاف تنسيقات الأرقام وتحويل قيم النص إلى قيم رقمية أو تاريخ/وقت للخلايا. سيُحافظ على هذا الإعداد للمصنف المُنشأ لاحقًا، أي أن [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) للمصنف سيستخدم نفس المنطقة مع هذه الخاصية.

**Returns:**
int
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


يضبط اسم الخط القياسي الافتراضي

**Remarks**

ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام DefaultStyleSettings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


يضبط حجم الخط القياسي الافتراضي.

**Remarks**

ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام DefaultStyleSettings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
double
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

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


يضبط خيارات الضبط التلقائي

**Remarks**

فقط لملف xlsx، spreadsheetML الآن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

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


يضبط قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


يضبط الترميز الافتراضي. ينطبق فقط على ملفات csv.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


يضبط إعدادات الخط الفردية. يعمل فقط مع الـ [Workbook](../../com.aspose.cells/workbook) الذي يستخدم هذا الـ [LoadOptions](../../com.aspose.cells/loadoptions) للتحميل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة.

**Remarks**

يعمل فقط لملفات xlsx، xlsb، و xlsm. هناك العديد من الأشكال المتداخلة المتطابقة التي لا فائدة منها في بعض الملفات، يمكننا تجاهلها عند تحميل الملفات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


يضبط مراقب المقاطعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

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

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


المرشح لتحديد كيفية تحميل البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


يشير إلى الاستراتيجية لتطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ/وقت.

انظر [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله.

**Remarks**

هذه الخاصية لها نفس التأثير مع [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) لتعيين الإعدادات الإقليمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Locale |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


يضبط وضع الذاكرة للمصنف المحمّل.

انظر [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

لمزيد من التفاصيل حول وضع الذاكرة، يرجى الاطلاع على [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


يضبط حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية.

**Remarks**

إذا لم يكن هناك إعداد لحجم الورق، سيستخدم MS Excel إعداد الطابعة الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). حجم الورق الافتراضي. |

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

بعد تحميل المصنف من ملف القالب باستخدام هذا الخيار، سيتم تعيين [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) إلى نفس القيمة مع هذه الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله.

انظر [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

قد تُستخدم الإعدادات الإقليمية لتهيئة بعض الميزات للمصنف مثل الخطوط والسمات وما إلى ذلك. بالنسبة لتنسيقات الملفات القائمة على النص، مثل CSV وHTML، ...، سيتم أيضًا استخدام الإعداد الإقليمي لاكتشاف تنسيقات الأرقام وتحويل قيم النص إلى قيم رقمية أو تاريخ/وقت للخلايا. سيُحافظ على هذا الإعداد للمصنف المُنشأ لاحقًا، أي أن [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) للمصنف سيستخدم نفس المنطقة مع هذه الخاصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


يضبط اسم الخط القياسي الافتراضي

**Remarks**

ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام DefaultStyleSettings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


يضبط حجم الخط القياسي الافتراضي.

**Remarks**

ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام DefaultStyleSettings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

