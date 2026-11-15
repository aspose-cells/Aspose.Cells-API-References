---
title: "فئة TxtLoadOptions"
linktitle: "TxtLoadOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة TxtLoadOptions. تغلف الكائن الذي يمثل txtloadoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/txtloadoptions/
---

## TxtLoadOptions class

يمثل الخيارات لتحميل ملف نصي.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewTxtLoadOptions](./newtxtloadoptions/) | ينشئ الخيارات لتحميل ملف نصي. |
| [NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | ينشئ الخيارات لتحميل ملف نصي. |
| [NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetSeparator](./getseparator/) | يحصل على ويضبط فاصل الأحرف لملف النص. |
| [SetSeparator](./setseparator/) | يحصل على ويضبط فاصل الأحرف لملف النص. |
| [GetSeparatorString](./getseparatorstring/) | يحصل على ويضبط قيمة سلسلة كفاصل. |
| [SetSeparatorString](./setseparatorstring/) | يحصل على ويضبط قيمة سلسلة كفاصل. |
| [IsMultiEncoded](./ismultiencoded/) | True يعني أن الملف يحتوي على عدة ترميزات. |
| [SetIsMultiEncoded](./setismultiencoded/) | True يعني أن الملف يحتوي على عدة ترميزات. |
| [GetHasFormula](./gethasformula/) | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [SetHasFormula](./sethasformula/) | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [GetHasTextQualifier](./gethastextqualifier/) | ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true. |
| [SetHasTextQualifier](./sethastextqualifier/) | ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true. |
| [GetTextQualifier](./gettextqualifier/) | يحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو '"'. |
| [SetTextQualifier](./settextqualifier/) | يحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو '"'. |
| [GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | ما إذا كان يجب اعتبار الفواصل المتتالية كواحدة. |
| [SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | ما إذا كان يجب اعتبار الفواصل المتتالية كواحدة. |
| [GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | يشير إلى ما إذا كان يجب أخذ علامة الاقتباس المفردة الأولية كجزء من قيمة خلية واحدة. القيمة الافتراضية هي true. إذا كانت false، سيتم إزالة الاقتباس المفرد الأولي من قيمة الخلية المقابلة وسيتم ضبط Style.QuotePrefix كـ true للخلية. |
| [SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | يشير إلى ما إذا كان يجب أخذ علامة الاقتباس المفردة الأولية كجزء من قيمة خلية واحدة. القيمة الافتراضية هي true. إذا كانت false، سيتم إزالة الاقتباس المفرد الأولي من قيمة الخلية المقابلة وسيتم ضبط Style.QuotePrefix كـ true للخلية. |
| [GetExtendToNextSheet](./getextendtonextsheet/) | ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد. القيمة الافتراضية هي false. |
| [SetExtendToNextSheet](./setextendtonextsheet/) | ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد. القيمة الافتراضية هي false. |
| [GetHeaderRowsCount](./getheaderrowscount/) | عدد صفوف الرأس التي سيتم تكرارها للورقات الموسعة. |
| [SetHeaderRowsCount](./setheaderrowscount/) | عدد صفوف الرأس التي سيتم تكرارها للورقات الموسعة. |
| [GetHeaderColumnsCount](./getheadercolumnscount/) | عدد أعمدة الرأس التي يجب تكرارها للأوراق الموسعة. |
| [SetHeaderColumnsCount](./setheadercolumnscount/) | عدد أعمدة الرأس التي يجب تكرارها للأوراق الموسعة. |
| [GetMaxRowCount](./getmaxrowcount/) | العدد الأقصى للصفوف التي يمكن استيرادها لورقة واحدة. |
| [SetMaxRowCount](./setmaxrowcount/) | العدد الأقصى للصفوف التي يمكن استيرادها لورقة واحدة. |
| [GetMaxColumnCount](./getmaxcolumncount/) | العدد الأقصى للأعمدة التي يمكن استيرادها لورقة واحدة. |
| [SetMaxColumnCount](./setmaxcolumncount/) | العدد الأقصى للأعمدة التي يمكن استيرادها لورقة واحدة. |
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
