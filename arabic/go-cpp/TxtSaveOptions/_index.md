---
title: "فئة TxtSaveOptions"
linktitle: "TxtSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة TxtSaveOptions. تغلف الكائن الذي يمثل txtsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

يمثل خيارات الحفظ لتنسيق csv/محدد بعلامات تبويب/تنسيق نصي آخر.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | ينشئ خيارات حفظ ملف نصي. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | ينشئ خيارات حفظ ملف نصي. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetSeparator](./getseparator/) | يحصل على ويضبط char Delimiter لملف النص. |
| [SetSeparator](./setseparator/) | يحصل على ويضبط char Delimiter لملف النص. |
| [GetSeparatorString](./getseparatorstring/) | يحصل على ويضبط قيمة سلسلة كفاصل. |
| [SetSeparatorString](./setseparatorstring/) | يحصل على ويضبط قيمة سلسلة كفاصل. |
| [GetEncoding](./getencoding/) | يحصل على ويضبط الترميز الافتراضي. |
| [SetEncoding](./setencoding/) | يحصل على ويضبط الترميز الافتراضي. |
| [GetQuoteType](./getquotetype/) | يحصل على أو يضبط طريقة اقتباس القيم في ملف النص المُصدّر. |
| [SetQuoteType](./setquotetype/) | يحصل على أو يضبط طريقة اقتباس القيم في ملف النص المُصدّر. |
| [GetFormatStrategy](./getformatstrategy/) | يحصل على ويضبط استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة. |
| [SetFormatStrategy](./setformatstrategy/) | يحصل على ويضبط استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | يشير إلى ما إذا كان يجب قص الصفوف والأعمدة الفارغة الأولية كما يفعل ms excel. القيمة الافتراضية هي true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | يشير إلى ما إذا كان يجب قص الصفوف والأعمدة الفارغة الأولية كما يفعل ms excel. القيمة الافتراضية هي true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | يشير إلى ما إذا كان يجب قص الخلايا الفارغة المتبقية في صف واحد. القيمة الافتراضية هي false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | يشير إلى ما إذا كان يجب قص الخلايا الفارغة المتبقية في صف واحد. القيمة الافتراضية هي false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | يشير إلى ما إذا كان يجب إخراج الفواصل للصف الفارغ. القيمة الافتراضية هي false لذا سيكون محتوى الصف الفارغ فارغًا بشكل افتراضي. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | يشير إلى ما إذا كان يجب إخراج الفواصل للصف الفارغ. القيمة الافتراضية هي false لذا سيكون محتوى الصف الفارغ فارغًا بشكل افتراضي. |
| [GetExportArea](./getexportarea/) | نطاق الخلايا التي سيتم تصديرها. |
| [SetExportArea](./setexportarea/) | نطاق الخلايا التي سيتم تصديرها. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | يشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفرد كجزء من قيمة خلية واحدة عندما تكون Style.QuotePrefix صحيحة لها. القيمة الافتراضية هي false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | يشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفرد كجزء من قيمة خلية واحدة عندما تكون Style.QuotePrefix صحيحة لها. القيمة الافتراضية هي false. |
| [GetExportAllSheets](./getexportallsheets/) | يشير إلى ما إذا كان يجب تصدير جميع الأوراق إلى ملف النص. إذا كانت false، يتم تصدير الورقة النشطة فقط، كما في MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | يشير إلى ما إذا كان يجب تصدير جميع الأوراق إلى ملف النص. إذا كانت false، يتم تصدير الورقة النشطة فقط، كما في MS Excel. |
| [GetSaveFormat](./getsaveformat/) | يحصل على تنسيق ملف الحفظ. |
| [GetClearData](./getcleardata/) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [SetClearData](./setcleardata/) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [GetCachedFileFolder](./getcachedfilefolder/) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. |
| [SetCachedFileFolder](./setcachedfilefolder/) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [GetMergeAreas](./getmergeareas/) | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [SetMergeAreas](./setmergeareas/) | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [GetCreateDirectory](./getcreatedirectory/) | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [SetCreateDirectory](./setcreatedirectory/) | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [GetSortNames](./getsortnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [SetSortNames](./setsortnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [GetSortExternalNames](./getsortexternalnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [SetSortExternalNames](./setsortexternalnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [GetRefreshChartCache](./getrefreshchartcache/) | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [SetRefreshChartCache](./setrefreshchartcache/) | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت، سيتم قطعها. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت، سيتم قطعها. |
| [GetUpdateSmartArt](./getupdatesmartart/) | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. |
