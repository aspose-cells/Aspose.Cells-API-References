---
title: "JsonSaveOptions Class"
linktitle: "JsonSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "JsonSaveOptions class. يغلف الكائن الذي يمثل jsonsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

يمثل خيارات حفظ المصنف كملف JSON.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | ينشئ خيارات لحفظ ملف json. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetExportStylePool](./getexportstylepool/) | يشير إلى ما إذا كان يجب تصدير الأنماط جماعيًا أو فرديًا إلى كل خلية. |
| [SetExportStylePool](./setexportstylepool/) | يشير إلى ما إذا كان يجب تصدير الأنماط جماعيًا أو فرديًا إلى كل خلية. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | يمثل نوع تصدير الارتباط التشعبي إلى json. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | يمثل نوع تصدير الارتباط التشعبي إلى json. |
| [GetSkipEmptyRows](./getskipemptyrows/) | يشير إلى ما إذا كان يتم تخطي الصفوف الفارغة. |
| [SetSkipEmptyRows](./setskipemptyrows/) | يشير إلى ما إذا كان يتم تخطي الصفوف الفارغة. |
| [GetSheetIndexes](./getsheetindexes/) | يمثل فهارس الأوراق المصدرة. |
| [SetSheetIndexes](./setsheetindexes/) | يمثل فهارس الأوراق المصدرة. |
| [GetSchemas](./getschemas/) | مخطط json الأصلي لكل ورقة عمل. |
| [SetSchemas](./setschemas/) | مخطط json الأصلي لكل ورقة عمل. |
| [GetExportArea](./getexportarea/) | يحصل أو يضبط نطاق التصدير. |
| [SetExportArea](./setexportarea/) | يحصل أو يضبط نطاق التصدير. |
| [GetHasHeaderRow](./gethasheaderrow/) | يشير إلى ما إذا كان النطاق يحتوي على صف الرأس. |
| [SetHasHeaderRow](./sethasheaderrow/) | يشير إلى ما إذا كان النطاق يحتوي على صف الرأس. |
| [GetExportAsString](./getexportasstring/) | يصدّر قيمة السلسلة للخلية إلى json. |
| [SetExportAsString](./setexportasstring/) | يصدّر قيمة السلسلة للخلية إلى json. |
| [GetIndent](./getindent/) | يشير إلى المسافة البادئة. |
| [SetIndent](./setindent/) | يشير إلى المسافة البادئة. |
| [GetExportNestedStructure](./getexportnestedstructure/) | تم تصديره كهيكل Json هرمي أب-ابن. |
| [SetExportNestedStructure](./setexportnestedstructure/) | تم تصديره كهيكل Json هرمي أب-ابن. |
| [GetExportEmptyCells](./getexportemptycells/) | يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null. |
| [SetExportEmptyCells](./setexportemptycells/) | يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | يشير إلى ما إذا كان يتم دائمًا تصدير Excel إلى json ككائن، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | يشير إلى ما إذا كان يتم دائمًا تصدير Excel إلى json ككائن، حتى إذا كان هناك ورقة عمل واحدة فقط في الملف. |
| [GetToExcelStruct](./gettoexcelstruct/) | يشير إلى ما إذا كان يتم التحويل إلى بنية json لملف Excel. |
| [SetToExcelStruct](./settoexcelstruct/) | يشير إلى ما إذا كان يتم التحويل إلى بنية json لملف Excel. |
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
