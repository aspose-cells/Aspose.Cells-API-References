---
title: "فئة PptxSaveOptions"
linktitle: "PptxSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PptxSaveOptions. تغلف الكائن الذي يمثل pptxsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/pptxsaveoptions/
---

## PptxSaveOptions class

يمثل خيارات حفظ pptx.

```go

type PptxSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPptxSaveOptions](./newpptxsaveoptions/) | يمثل خيارات حفظ pptx. |
| [NewPptxSaveOptions_Bool](./newpptxsaveoptions_bool/) | يمثل خيارات حفظ ملف .pptx. |
| [NewPptxSaveOptions_PaginatedSaveOptions](./newpptxsaveoptions_paginatedsaveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetIgnoreHiddenRows](./getignorehiddenrows/) | يشير إلى ما إذا كان يتم تجاهل الصفوف المخفية عند تحويل Excel إلى PowerPoint. |
| [SetIgnoreHiddenRows](./setignorehiddenrows/) | يشير إلى ما إذا كان يتم تجاهل الصفوف المخفية عند تحويل Excel إلى PowerPoint. |
| [GetSaveAsEditableShapes](./getsaveaseditableshapes/) | احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف pptx، حتى تتمكن من تعديلها في PowerPoint. |
| [SetSaveAsEditableShapes](./setsaveaseditableshapes/) | احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف pptx، حتى تتمكن من تعديلها في PowerPoint. |
| [GetEmbedXlsxAsChartDataSource](./getembedxlsxaschartdatasource/) | يشير إلى ما إذا كان سيتم تضمين ملف xlsx كمصدر بيانات للمخطط. |
| [SetEmbedXlsxAsChartDataSource](./setembedxlsxaschartdatasource/) | يشير إلى ما إذا كان سيتم تضمين ملف xlsx كمصدر بيانات للمخطط. |
| [GetAdjustFontSizeForRowType](./getadjustfontsizeforrowtype/) | يمثل نوع الخط الذي يحتاج إلى تعديل حجم الخط إذا كان ارتفاع الصف صغيرًا. |
| [SetAdjustFontSizeForRowType](./setadjustfontsizeforrowtype/) | يمثل نوع الخط الذي يحتاج إلى تعديل حجم الخط إذا كان ارتفاع الصف صغيرًا. |
| [GetExportViewType](./getexportviewtype/) | يحصل على نوع العرض ويضبطه عند التصدير إلى PowerPoint. نوع التصدير الافتراضي يعمل كطباعة. |
| [SetExportViewType](./setexportviewtype/) | يحصل على نوع العرض ويضبطه عند التصدير إلى PowerPoint. نوع التصدير الافتراضي يعمل كطباعة. |
| [GetAsFlatOpc](./getasflatopc/) | يشير إلى ما إذا كان سيتم الحفظ كملف opc مسطح يمكن إنشاؤه بواسطة Open XML SDK. |
| [SetAsFlatOpc](./setasflatopc/) | يشير إلى ما إذا كان سيتم الحفظ كملف opc مسطح يمكن إنشاؤه بواسطة Open XML SDK. |
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
