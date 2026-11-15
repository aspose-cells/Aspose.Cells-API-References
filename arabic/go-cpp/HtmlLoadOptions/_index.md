---
title: "فئة HtmlLoadOptions"
linktitle: "HtmlLoadOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "الفئة HtmlLoadOptions. تغلف الكائن الذي يمثل htmlloadoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/htmlloadoptions/
---

## HtmlLoadOptions class

يمثل الخيارات عند استيراد ملف HTML.

```go

type HtmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewHtmlLoadOptions](./newhtmlloadoptions/) | ينشئ خيارات تحميل الملف. |
| [NewHtmlLoadOptions_LoadFormat](./newhtmlloadoptions_loadformat/) | ينشئ خيارات تحميل الملف. |
| [NewHtmlLoadOptions_AbstractTextLoadOptions](./newhtmlloadoptions_abstracttextloadoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetLoadFormulas](./getloadformulas/) | يشير إلى ما إذا كان يتم استيراد الصيغ إذا كان ملف html الأصلي يحتوي على صيغ. |
| [SetLoadFormulas](./setloadformulas/) | يشير إلى ما إذا كان يتم استيراد الصيغ إذا كان ملف html الأصلي يحتوي على صيغ. |
| [GetSupportDivTag](./getsupportdivtag/) | يشير إلى ما إذا كان يدعم تخطيط الوسم <c>&lt;div&gt;</c> عندما يحتوي ملف html عليه. القيمة الافتراضية هي false. |
| [SetSupportDivTag](./setsupportdivtag/) | يشير إلى ما إذا كان يدعم تخطيط الوسم <c>&lt;div&gt;</c> عندما يحتوي ملف html عليه. القيمة الافتراضية هي false. |
| [GetDeleteRedundantSpaces](./getdeleteredundantspaces/) | يشير إلى ما إذا كان يحذف المسافات الزائدة عندما يلتف النص إلى أسطر باستخدام وسم <c>&lt;br&gt;</c>. القيمة الافتراضية هي false. |
| [SetDeleteRedundantSpaces](./setdeleteredundantspaces/) | يشير إلى ما إذا كان يحذف المسافات الزائدة عندما يلتف النص إلى أسطر باستخدام وسم <c>&lt;br&gt;</c>. القيمة الافتراضية هي false. |
| [GetAutoFitColsAndRows](./getautofitcolsandrows/) | يشير إلى ما إذا كان يتم ضبط الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي false. |
| [SetAutoFitColsAndRows](./setautofitcolsandrows/) | يشير إلى ما إذا كان يتم ضبط الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي false. |
| [GetHasFormula](./gethasformula/) | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [SetHasFormula](./sethasformula/) | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [GetProgId](./getprogid/) | يحصل على معرف البرنامج لإنشاء الملف. يقتصر على ملفات MHT. |
| [GetTableLoadOptions](./gettableloadoptions/) | احصل على كائن HtmlTableLoadOptionCollection |
| [GetDetectLaTeX](./getdetectlatex/) | يشير إلى ما إذا كان سيتم اكتشاف صيغ LaTeX في ملف HTML. القيمة الافتراضية هي false. |
| [SetDetectLaTeX](./setdetectlatex/) | يشير إلى ما إذا كان سيتم اكتشاف صيغ LaTeX في ملف HTML. القيمة الافتراضية هي false. |
| [GetParagraphLayoutMode](./getparagraphlayoutmode/) | يحدد كيفية عرض عناصر HTML &lt;p&gt; عند تحميل HTML. القيمة الافتراضية هي HtmlParagraphLayoutMode.Normal. |
| [SetParagraphLayoutMode](./setparagraphlayoutmode/) | يحدد كيفية عرض عناصر HTML &lt;p&gt; عند تحميل HTML. القيمة الافتراضية هي HtmlParagraphLayoutMode.Normal. |
| [GetHyperlinkLoadMode](./gethyperlinkloadmode/) | يحدد كيفية تحميل الروابط التشعبية عند تحميل HTML. |
| [SetHyperlinkLoadMode](./sethyperlinkloadmode/) | يحدد كيفية تحميل الروابط التشعبية عند تحميل HTML. |
| [GetEncoding](./getencoding/) | يحصل على الترميز الافتراضي ويضبطه. ينطبق فقط على ملفات csv. |
| [SetEncoding](./setencoding/) | يحصل على الترميز الافتراضي ويضبطه. ينطبق فقط على ملفات csv. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | يشير إلى الاستراتيجية لتطبيق النمط على القيم المُحللة عند تحويل قيمة النص إلى رقم أو تاريخ/وقت. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | يشير إلى الاستراتيجية لتطبيق النمط على القيم المُحللة عند تحويل قيمة النص إلى رقم أو تاريخ/وقت. |
| [GetConvertNumericData](./getconvertnumericdata/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان النص في ملف النص يُحول إلى بيانات رقمية. القيمة الافتراضية هي true. |
| [SetConvertNumericData](./setconvertnumericdata/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان النص في ملف النص يُحول إلى بيانات رقمية. القيمة الافتراضية هي true. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان النص في ملف النص يُحول إلى بيانات تاريخية. القيمة الافتراضية هي true. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان النص في ملف النص يُحول إلى بيانات تاريخية. القيمة الافتراضية هي true. |
| [GetKeepPrecision](./getkeepprecision/) | يشير إلى عدم تحليل قيمة النص إذا كان طولها 15. |
| [SetKeepPrecision](./setkeepprecision/) | يشير إلى عدم تحليل قيمة النص إذا كان طولها 15. |
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
