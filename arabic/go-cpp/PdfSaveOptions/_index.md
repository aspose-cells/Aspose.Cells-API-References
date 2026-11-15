---
title: "فئة PdfSaveOptions"
linktitle: "PdfSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PdfSaveOptions. تغلف الكائن الذي يمثل pdfsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/pdfsaveoptions/
---

## PdfSaveOptions class

يمثل خيارات حفظ ملف pdf.

```go

type PdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPdfSaveOptions](./newpdfsaveoptions/) | ينشئ الخيارات لحفظ ملف PDF. |
| [NewPdfSaveOptions_PaginatedSaveOptions](./newpdfsaveoptions_paginatedsaveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetEmbedStandardWindowsFonts](./getembedstandardwindowsfonts/) | True لتضمين خطوط TrueType. يؤثر فقط على أحرف ASCII 32-127. الخطوط للأكواد التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط يتم تضمينها دائمًا لمعيار PDF/A-1a و PDF/A-1b. القيمة الافتراضية هي true. |
| [SetEmbedStandardWindowsFonts](./setembedstandardwindowsfonts/) | True لتضمين خطوط TrueType. يؤثر فقط على أحرف ASCII 32-127. الخطوط للأكواد التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط يتم تضمينها دائمًا لمعيار PDF/A-1a و PDF/A-1b. القيمة الافتراضية هي true. |
| [GetBookmark](./getbookmark/) | يحصل على ويضبط كائن PdfBookmarkEntry</see>. |
| [SetBookmark](./setbookmark/) | يحصل على ويضبط كائن PdfBookmarkEntry</see>. |
| [GetCompliance](./getcompliance/) | يحصل على أو يضبط مستوى التوافق مع معايير PDF للمستندات الناتجة. |
| [SetCompliance](./setcompliance/) | يحصل على أو يضبط مستوى التوافق مع معايير PDF للمستندات الناتجة. |
| [GetSecurityOptions](./getsecurityoptions/) | عيّن هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf. |
| [SetSecurityOptions](./setsecurityoptions/) | عيّن هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf. |
| [GetCalculateFormula](./getcalculateformula/) | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF. |
| [SetCalculateFormula](./setcalculateformula/) | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF. |
| [GetPdfCompression](./getpdfcompression/) | حدد خوارزمية الضغط |
| [SetPdfCompression](./setpdfcompression/) | حدد خوارزمية الضغط |
| [SetImageResample](./setimageresample/) | يضبط PPI (بكسل لكل بوصة) المطلوب لإعادة تحجيم الصور وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG بالإعداد المحدد للجودة، وستُعاد تحجيم الصور التي تتجاوز الـ PPI المحدد. |
| [GetCreatedTime](./getcreatedtime/) | يحصل على ويضبط وقت إنشاء مستند PDF. |
| [SetCreatedTime](./setcreatedtime/) | يحصل على ويضبط وقت إنشاء مستند PDF. |
| [GetProducer](./getproducer/) | يحصل على ويضبط المنتج (producer) لمستند PDF المُنشأ. |
| [SetProducer](./setproducer/) | يحصل على ويضبط المنتج (producer) لمستند PDF المُنشأ. |
| [GetOptimizationType](./getoptimizationtype/) | يحصل على ويضبط نوع تحسين PDF. |
| [SetOptimizationType](./setoptimizationtype/) | يحصل على ويضبط نوع تحسين PDF. |
| [GetCustomPropertiesExport](./getcustompropertiesexport/) | يحصل على أو يضبط قيمة تحدد طريقة تصدير CustomDocumentPropertyCollection إلى ملف PDF. القيمة الافتراضية هي None. |
| [SetCustomPropertiesExport](./setcustompropertiesexport/) | يحصل على أو يضبط قيمة تحدد طريقة تصدير CustomDocumentPropertyCollection إلى ملف PDF. القيمة الافتراضية هي None. |
| [GetExportDocumentStructure](./getexportdocumentstructure/) | يشير إلى ما إذا كان يجب تصدير بنية المستند. |
| [SetExportDocumentStructure](./setexportdocumentstructure/) | يشير إلى ما إذا كان يجب تصدير بنية المستند. |
| [GetDisplayDocTitle](./getdisplaydoctitle/) | يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند. |
| [SetDisplayDocTitle](./setdisplaydoctitle/) | يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند. |
| [GetFontEncoding](./getfontencoding/) | يحصل على أو يضبط ترميز الخط المضمّن في PDF. |
| [SetFontEncoding](./setfontencoding/) | يحصل على أو يضبط ترميز الخط المضمّن في PDF. |
| [GetWatermark](./getwatermark/) | يحصل أو يضبط العلامة المائية للإخراج. |
| [SetWatermark](./setwatermark/) | يحصل أو يضبط العلامة المائية للإخراج. |
| [GetEmbedAttachments](./getembedattachments/) | يشير إلى ما إذا كان يجب تضمين المرفق لكائنات Ole في Excel. |
| [SetEmbedAttachments](./setembedattachments/) | يشير إلى ما إذا كان يجب تضمين المرفق لكائنات Ole في Excel. |
| [GetZoomBehavior](./getzoombehavior/) | يحصل أو يضبط وضع العرض الأولي عند فتح مستند PDF المُنشأ. القيمة الافتراضية هي PdfZoomBehavior.None. |
| [SetZoomBehavior](./setzoombehavior/) | يحصل أو يضبط وضع العرض الأولي عند فتح مستند PDF المُنشأ. القيمة الافتراضية هي PdfZoomBehavior.None. |
| [GetZoomFactor](./getzoomfactor/) | يحصل أو يضبط نسبة التكبير المستخدمة عندما يكون ZoomBehavior هو PdfZoomBehavior.ZoomFactor. |
| [SetZoomFactor](./setzoomfactor/) | يحصل أو يضبط نسبة التكبير المستخدمة عندما يكون ZoomBehavior هو PdfZoomBehavior.ZoomFactor. |
| [GetDefaultFont](./getdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود. |
| [SetDefaultFont](./setdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [GetOnePagePerSheet](./getonepagepersheet/) | إذا كان OnePagePerSheet يساوي true، سيتم إخراج كل محتوى ورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون حجم الورق في إعدادات الصفحة غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [SetOnePagePerSheet](./setonepagepersheet/) | إذا كان OnePagePerSheet يساوي true، سيتم إخراج كل محتوى ورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون حجم الورق في إعدادات الصفحة غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | إذا كان AllColumnsInOnePagePerSheet يساوي true، سيتم إخراج كل محتوى الأعمدة في ورقة واحدة في صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعدادات الصفحة، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | إذا كان AllColumnsInOnePagePerSheet يساوي true، سيتم إخراج كل محتوى الأعمدة في ورقة واحدة في صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعدادات الصفحة، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [GetIgnoreError](./getignoreerror/) | يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء التصيير. قد يكون الخطأ في الشكل أو الصورة أو تصيير المخطط، إلخ. |
| [SetIgnoreError](./setignoreerror/) | يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء التصيير. قد يكون الخطأ في الشكل أو الصورة أو تصيير المخطط، إلخ. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة. |
| [SetPageIndex](./setpageindex/) | يحصل أو يعيّن الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [GetPageIndex](./getpageindex/) | يحصل أو يعيّن الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [SetPageCount](./setpagecount/) | يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. |
| [GetPageCount](./getpagecount/) | يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. |
| [GetPrintingPageType](./getprintingpagetype/) | يشير إلى الصفحات التي لن تُطبع. |
| [SetPrintingPageType](./setprintingpagetype/) | يشير إلى الصفحات التي لن تُطبع. |
| [GetGridlineType](./getgridlinetype/) | يحصل أو يعيّن نوع خطوط الشبكة. |
| [SetGridlineType](./setgridlinetype/) | يحصل أو يعيّن نوع خطوط الشبكة. |
| [GetGridlineColor](./getgridlinecolor/) | يحصل أو يعيّن لون خطوط الشبكة. |
| [SetGridlineColor](./setgridlinecolor/) | يحصل أو يعيّن لون خطوط الشبكة. |
| [GetTextCrossType](./gettextcrosstype/) | يحصل أو يعيّن نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [SetTextCrossType](./settextcrosstype/) | يحصل أو يعيّن نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | يحصل أو يعيّن لغة التحرير الافتراضية. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | يحصل أو يعيّن لغة التحرير الافتراضية. |
| [GetSheetSet](./getsheetset/) | يحصل أو يعيّن الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | يحصل أو يعيّن الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | يطبق هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | يطبق هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [GetEmfRenderSetting](./getemfrendersetting/) | إعداد لتصوير ملف Emf الميتا. |
| [SetEmfRenderSetting](./setemfrendersetting/) | إعداد لتصوير ملف Emf الميتا. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | يحصل أو يعيّن الإعدادات المخصصة أثناء التصيير. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | يحصل أو يعيّن الإعدادات المخصصة أثناء التصيير. |
| [GetRenderingBehavior](./getrenderingbehavior/) | يحصل أو يعيّن سلوكيات التصيير الخاصة بـ Excel لتطبيقها. |
| [SetRenderingBehavior](./setrenderingbehavior/) | يحصل أو يعيّن سلوكيات التصيير الخاصة بـ Excel لتطبيقها. |
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
