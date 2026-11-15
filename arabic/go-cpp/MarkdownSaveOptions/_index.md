---
title: "فئة MarkdownSaveOptions"
linktitle: "MarkdownSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة MarkdownSaveOptions. تغلف الكائن الذي يمثل markdownsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

يمثل خيارات الحفظ لـ markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | ينشئ خيارات لحفظ مستند markdown |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetEncoding](./getencoding/) | يحصل على ويضبط الترميز الافتراضي. |
| [SetEncoding](./setencoding/) | يحصل على ويضبط الترميز الافتراضي. |
| [GetFormatStrategy](./getformatstrategy/) | يحصل على ويضبط استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة. |
| [SetFormatStrategy](./setformatstrategy/) | يحصل على ويضبط استراتيجية التنسيق عند تصدير قيمة الخلية كسلسلة. |
| [GetLineSeparator](./getlineseparator/) | يحصل ويضبط فاصل السطر. |
| [SetLineSeparator](./setlineseparator/) | يحصل ويضبط فاصل السطر. |
| [GetTableHeaderType](./gettableheadertype/) | يحصل ويضبط طريقة تعيين رأس الجدول. |
| [SetTableHeaderType](./settableheadertype/) | يحصل ويضبط طريقة تعيين رأس الجدول. |
| [GetSheetSet](./getsheetset/) | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | احصل على كائن ImageOrPrintOptions قبل التصدير |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى Markdown. القيمة الافتراضية هي true. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى Markdown. القيمة الافتراضية هي true. |
| [GetCalculateFormula](./getcalculateformula/) | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف markdown. |
| [SetCalculateFormula](./setcalculateformula/) | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف markdown. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | يشير إلى ما إذا كان يجب تصدير الروابط باستخدام تعريفات المرجعية بدلاً من الصيغة المضمنة. القيمة الافتراضية هي false. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | يشير إلى ما إذا كان يجب تصدير الروابط باستخدام تعريفات المرجعية بدلاً من الصيغة المضمنة. القيمة الافتراضية هي false. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | يشير إلى ما إذا كان محاذاة الأعمدة مفعّلة للجداول Markdown المُولدة. عندما تكون مفعّلة، يتم محاذاة الأعمدة بملء محتوى الخلية بالحرف المحدد (عادةً ' ' للمسافات). اضبطه على '\0' لتعطيل محاذاة الأعمدة (الافتراضي). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | يشير إلى ما إذا كان محاذاة الأعمدة مفعّلة للجداول Markdown المُولدة. عندما تكون مفعّلة، يتم محاذاة الأعمدة بملء محتوى الخلية بالحرف المحدد (عادةً ' ' للمسافات). اضبطه على '\0' لتعطيل محاذاة الأعمدة (الافتراضي). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | يشير إلى ما إذا كان يجب اعتبار الصفوف الفارغة في ورقة العمل كفواصل للجداول عند التصدير إلى Markdown. القيمة الافتراضية هي false. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | يشير إلى ما إذا كان يجب اعتبار الصفوف الفارغة في ورقة العمل كفواصل للجداول عند التصدير إلى Markdown. القيمة الافتراضية هي false. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | يشير إلى كيفية تصدير كائنات OfficeMath إلى Markdown، القيمة الافتراضية هي Image. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | يشير إلى كيفية تصدير كائنات OfficeMath إلى Markdown، القيمة الافتراضية هي Image. |
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
