---
title: "فئة OdsLoadOptions"
linktitle: "OdsLoadOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة OdsLoadOptions. يحتوي على الكائن الذي يمثل odsloadoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/odsloadoptions/
---

## OdsLoadOptions class

يمثل خيارات تحميل ملف ods.

```go

type OdsLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewOdsLoadOptions](./newodsloadoptions/) | يمثل خيارات تحميل ملف ods. |
| [NewOdsLoadOptions_LoadFormat](./newodsloadoptions_loadformat/) | يمثل خيارات تحميل ملف ods. |
| [NewOdsLoadOptions_LoadOptions](./newodsloadoptions_loadoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetApplyExcelDefaultStyleToHyperlink](./getapplyexceldefaultstyletohyperlink/) | يشير إلى ما إذا كان يتم تطبيق النمط الافتراضي لبرنامج Excel على الارتباط التشعبي. |
| [SetApplyExcelDefaultStyleToHyperlink](./setapplyexceldefaultstyletohyperlink/) | يشير إلى ما إذا كان يتم تطبيق النمط الافتراضي لبرنامج Excel على الارتباط التشعبي. |
| [GetRefreshPivotTables](./getrefreshpivottables/) | يشير إلى ما إذا كان يتم تحديث جداول pivot عند تحميل الملف. |
| [SetRefreshPivotTables](./setrefreshpivottables/) | يشير إلى ما إذا كان يتم تحديث جداول pivot عند تحميل الملف. |
| [IsClassicPivotTable](./isclassicpivottable/) | يشير إلى ما إذا كانت جدول pivot كلاسيكي. |
| [SetIsClassicPivotTable](./setisclassicpivottable/) | يشير إلى ما إذا كانت جدول pivot كلاسيكي. |
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
