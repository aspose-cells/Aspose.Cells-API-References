---
title: "فئة OoxmlSaveOptions"
linktitle: "OoxmlSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة OoxmlSaveOptions. تغلف الكائن الذي يمثل ooxmlsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

يمثل خيارات حفظ ملف Office Open XML.

```go

type OoxmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewOoxmlSaveOptions](./newooxmlsaveoptions/) | ينشئ الخيارات لحفظ ملف Office Open XML. |
| [NewOoxmlSaveOptions_SaveFormat](./newooxmlsaveoptions_saveformat/) | ينشئ الخيارات لحفظ ملف Office Open XML. |
| [NewOoxmlSaveOptions_SaveOptions](./newooxmlsaveoptions_saveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetAsFlatOpc](./getasflatopc/) | يشير إلى ما إذا كان يتم الحفظ كملف opc مسطح يمكن توليده بواسطة Open XML SDK. |
| [SetAsFlatOpc](./setasflatopc/) | يشير إلى ما إذا كان يتم الحفظ كملف opc مسطح يمكن توليده بواسطة Open XML SDK. |
| [GetExportCellName](./getexportcellname/) | يشير إلى ما إذا كان يتم تصدير اسم الخلية إلى ملف Excel2007 .xlsx (.xlsm, .xltx, .xltm). إذا كان من الممكن الوصول إلى ملف الإخراج بواسطة SQL Server DTS، يجب أن تكون هذه القيمة true. ضبط القيمة على false سيزيد الأداء بشكل كبير ويقلل حجم الملف عند إنشاء ملفات كبيرة. القيمة الافتراضية هي true. |
| [SetExportCellName](./setexportcellname/) | يشير إلى ما إذا كان يتم تصدير اسم الخلية إلى ملف Excel2007 .xlsx (.xlsm, .xltx, .xltm). إذا كان من الممكن الوصول إلى ملف الإخراج بواسطة SQL Server DTS، يجب أن تكون هذه القيمة true. ضبط القيمة على false سيزيد الأداء بشكل كبير ويقلل حجم الملف عند إنشاء ملفات كبيرة. القيمة الافتراضية هي true. |
| [GetUpdateZoom](./getupdatezoom/) | يشير إلى ما إذا كان يتم تحديث عامل القياس قبل حفظ الملف إذا كانت خصائص PageSetup.FitToPagesWide و PageSetup.FitToPagesTall تتحكم في كيفية تحجيم ورقة العمل. |
| [SetUpdateZoom](./setupdatezoom/) | يشير إلى ما إذا كان يتم تحديث عامل القياس قبل حفظ الملف إذا كانت خصائص PageSetup.FitToPagesWide و PageSetup.FitToPagesTall تتحكم في كيفية تحجيم ورقة العمل. |
| [GetEnableZip64](./getenablezip64/) | استخدم امتدادات ZIP64 عند كتابة أرشيفات zip حسب الحاجة. |
| [SetEnableZip64](./setenablezip64/) | استخدم امتدادات ZIP64 عند كتابة أرشيفات zip حسب الحاجة. |
| [GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | يشير إلى ما إذا كان يتم تضمين ملفات Ooxml لكائن OleObject ككائن ole. |
| [SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | يشير إلى ما إذا كان يتم تضمين ملفات Ooxml لكائن OleObject ككائن ole. |
| [GetCompressionType](./getcompressiontype/) | يحصل ويضبط نوع الضغط لملف ooxml. |
| [SetCompressionType](./setcompressiontype/) | يحصل ويضبط نوع الضغط لملف ooxml. |
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
