---
title: "NumbersLoadOptions فئة"
linktitle: "NumbersLoadOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة NumbersLoadOptions. يغلف الكائن الذي يمثل numbersloadoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/numbersloadoptions/
---

## NumbersLoadOptions class

يمثل خيارات تحميل ملفات Apple Numbers.

```go

type NumbersLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewNumbersLoadOptions](./newnumbersloadoptions/) | منشئ. |
| [NewNumbersLoadOptions_LoadOptions](./newnumbersloadoptions_loadoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetPreserveTableName](./getpreservetablename/) | يشير إلى ما إذا كان يجب الحفاظ على أسماء الجداول عند الاستيراد من Numbers. |
| [SetPreserveTableName](./setpreservetablename/) | يشير إلى ما إذا كان يجب الحفاظ على أسماء الجداول عند الاستيراد من Numbers. |
| [GetLoadTableType](./getloadtabletype/) | يحصل ويضبط نوع تحميل جداول متعددة في ورقة عمل واحدة. |
| [SetLoadTableType](./setloadtabletype/) | يحصل ويضبط نوع تحميل جداول متعددة في ورقة عمل واحدة. |
| [GetLoadFormat](./getloadformat/) | يحصل على تنسيق التحميل. |
| [GetPassword](./getpassword/) | يحصل على كلمة مرور المصنف ويضبطها. |
| [SetPassword](./setpassword/) | يحصل على كلمة مرور المصنف ويضبطها. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false. |
| [SetPaperSize](./setpapersize/) | يضبط حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية. |
| [GetLanguageCode](./getlanguagecode/) | يحصل على أو يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على رمز البلد (CountryCode) الذي تم حفظ الملف به. |
| [SetLanguageCode](./setlanguagecode/) | يحصل على أو يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على رمز البلد (CountryCode) الذي تم حفظ الملف به. |
| [GetRegion](./getregion/) | يحصل على أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله. |
| [SetRegion](./setregion/) | يحصل على أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط المصنف. |
| [GetInterruptMonitor](./getinterruptmonitor/) | يحصل على أو يضبط مراقب المقاطعة. |
| [SetInterruptMonitor](./setinterruptmonitor/) | يحصل على أو يضبط مراقب المقاطعة. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً. |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً. |
| [GetCheckDataValid](./getcheckdatavalid/) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [SetCheckDataValid](./setcheckdatavalid/) | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة السلسلة التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة السلسلة التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة للملفات الأخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true. |
| [GetLoadFilter](./getloadfilter/) | المرشح لتحديد طريقة تحميل البيانات. |
| [SetLoadFilter](./setloadfilter/) | المرشح لتحديد طريقة تحميل البيانات. |
| [GetMemorySetting](./getmemorysetting/) | يحصل على أو يضبط وضع الذاكرة للمصنف المحمل. |
| [SetMemorySetting](./setmemorysetting/) | يحصل على أو يضبط وضع الذاكرة للمصنف المحمل. |
| [GetAutoFitterOptions](./getautofitteroptions/) | يحصل على أو يضبط خيارات الضبط التلقائي. |
| [SetAutoFitterOptions](./setautofitteroptions/) | يحصل على أو يضبط خيارات الضبط التلقائي. |
| [GetAutoFilter](./getautofilter/) | يشير إلى ما إذا كان يتم تطبيق الترشيح التلقائي للبيانات عند تحميل الملفات. |
| [SetAutoFilter](./setautofilter/) | يشير إلى ما إذا كان يتم تطبيق الترشيح التلقائي للبيانات عند تحميل الملفات. |
| [GetFontConfigs](./getfontconfigs/) | يحصل على أو يضبط إعدادات الخط الفردية. يعمل فقط مع المصنف الذي يستخدم هذه LoadOptions للتحميل. |
| [SetFontConfigs](./setfontconfigs/) | يحصل على أو يضبط إعدادات الخط الفردية. يعمل فقط مع المصنف الذي يستخدم هذه LoadOptions للتحميل. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة عند الحصول على الصيغ وضبطها. القيمة الافتراضية هي false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تُضاف بين رموز الصيغة عند الحصول على الصيغ وضبطها. القيمة الافتراضية هي false. |
