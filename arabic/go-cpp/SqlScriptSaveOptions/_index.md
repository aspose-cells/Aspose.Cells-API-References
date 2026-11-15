---
title: "فئة SqlScriptSaveOptions"
linktitle: "SqlScriptSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة SqlScriptSaveOptions. تغلف الكائن الذي يمثل sqlscriptsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

يمثل خيارات حفظ sql.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | ينشئ خيارات لحفظ ملف sql. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء |
| [SetCheckIfTableExists](./setcheckiftableexists/) | تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء |
| [GetColumnTypeMap](./getcolumntypemap/) | يحصل ويضبط خريطة نوع العمود لمختلف قواعد البيانات. |
| [SetColumnTypeMap](./setcolumntypemap/) | يحصل ويضبط خريطة نوع العمود لمختلف قواعد البيانات. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | تحقق من جميع البيانات للعثور على نوع بيانات الأعمدة. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | تحقق من جميع البيانات للعثور على نوع بيانات الأعمدة. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | أدخل سطرًا فارغًا بين كل بيانات. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | أدخل سطرًا فارغًا بين كل بيانات. |
| [GetSeparator](./getseparator/) | يحصل ويضبط فاصل الأحرف لسكريبت sql. |
| [SetSeparator](./setseparator/) | يحصل ويضبط فاصل الأحرف لسكريبت sql. |
| [GetOperatorType](./getoperatortype/) | يحصل ويضبط نوع المشغل في sql. |
| [SetOperatorType](./setoperatortype/) | يحصل ويضبط نوع المشغل في sql. |
| [GetPrimaryKey](./getprimarykey/) | يمثل أي عمود هو المفتاح الأساسي لجدول البيانات. |
| [SetPrimaryKey](./setprimarykey/) | يمثل أي عمود هو المفتاح الأساسي لجدول البيانات. |
| [GetCreateTable](./getcreatetable/) | يشير إلى ما إذا كان يتم تصدير sql لإنشاء الجدول. |
| [SetCreateTable](./setcreatetable/) | يشير إلى ما إذا كان يتم تصدير sql لإنشاء الجدول. |
| [GetIdName](./getidname/) | يحصل ويضبط اسم عمود المعرف. |
| [SetIdName](./setidname/) | يحصل ويضبط اسم عمود المعرف. |
| [GetStartId](./getstartid/) | يحصل ويضبط معرف البداية. |
| [SetStartId](./setstartid/) | يحصل ويضبط معرف البداية. |
| [GetTableName](./gettablename/) | يحصل ويضبط اسم الجدول. |
| [SetTableName](./settablename/) | يحصل ويضبط اسم الجدول. |
| [GetExportAsString](./getexportasstring/) | يشير إلى ما إذا كان يتم تصدير جميع البيانات كقيمة نصية. |
| [SetExportAsString](./setexportasstring/) | يشير إلى ما إذا كان يتم تصدير جميع البيانات كقيمة نصية. |
| [GetSheetIndexes](./getsheetindexes/) | يمثل فهارس الأوراق المصدرة. |
| [SetSheetIndexes](./setsheetindexes/) | يمثل فهارس الأوراق المصدرة. |
| [GetExportArea](./getexportarea/) | يحصل أو يضبط نطاق التصدير. |
| [SetExportArea](./setexportarea/) | يحصل أو يضبط نطاق التصدير. |
| [GetHasHeaderRow](./gethasheaderrow/) | يشير إلى ما إذا كان النطاق يحتوي على صف الرأس. |
| [SetHasHeaderRow](./sethasheaderrow/) | يشير إلى ما إذا كان النطاق يحتوي على صف الرأس. |
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
