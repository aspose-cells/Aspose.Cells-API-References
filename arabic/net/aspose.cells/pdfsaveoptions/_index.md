---
title: PdfSaveOptions
second_title: Aspose.Cells لمرجع .NET API
description: يمثل خيارات حفظ ملف pdf.
type: docs
weight: 4500
url: /ar/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

يمثل خيارات حفظ ملف pdf.

```csharp
public class PdfSaveOptions : SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | ينشئ خيارات حفظ ملف pdf . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | إذا كانت AllColumnsInOnePagePerSheet صحيحة ، فسيتم إخراج كافة محتويات العمود في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق لإعداد الصفحات ، وستظل الإعدادات الأخرى لإعداد الصفحات سارية المفعول. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | يحصل على ملف[`Pdf المرجعية الدخول`](../../aspose.cells.rendering/pdfbookmarkentry) الكائن . |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | يتم استخدام مجلد الملف المخزن مؤقتًا لتخزين بعض البيانات الكبيرة. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | يشير إلى ما إذا كان سيتم حساب الصيغ قبل حفظ ملف pdf. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | يشير إلى ما إذا كان سيتم التحقق من توافق الخط لكل حرف في النص. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ، قد تظهر ككتلة في pdf ، image. اضبط هذا على "true" لمحاولة استخدام الخط الافتراضي للمصنف لإظهار هذه الأحرف أولاً. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | اجعل المصنف فارغًا بعد حفظ الملف. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | سيتم تحويل المصنف إلى pdf وفقًا لـ PdfCompliance في هذه الخاصية. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | إذا كان صحيحًا وكان الدليل غير موجود ، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | الحصول على وقت إنشاء مستند pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | الحصول على أو تعيين قيمة تحدد الطريقة[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) يتم تصديرها إلى ملف PDF. القيمة الافتراضية هي بلا. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | الحصول على لغة التحرير الافتراضية أو تعيينها. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ، قد تظهر ككتلة في ملف pdf ، image. قم بتعيين الخط الافتراضي مثل MingLiu أو MS Gothic لإظهار هذه الأحرف . إذا كانت هذه الخاصية هي لم يتم تعيينها ، ستستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار أحرف unicode هذه. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | يشير إلى ما إذا كان يجب أن يعرض شريط عنوان النافذة عنوان المستند. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | تنفيذ هذه الواجهة للحصول على DrawObject و Bound عند العرض. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | صحيح أن يتم تضمين خطوط كتابة صحيحة. يؤثر فقط على أحرف ASCII 32-127. يتم دائمًا تضمين خطوط رموز الأحرف الأكبر من 127. يتم دائمًا تضمين الخطوط لمعيار PDF / A-1a و PDF / A-1b . الافتراضي هو true . |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | إعداد عرض ملف تعريف Emf . |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | يشير إلى ما إذا كان سيتم تصدير بنية المستند. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | الحصول على أو تعيين ترميز الخط المضمن في ملف pdf. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | الحصول على نوع خط الشبكة أو تعيينه. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء العرض. يمكن أن يكون الخطأ خطأ في الشكل أو الصورة أو عرض المخطط ، إلخ. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | يشير إلى ما إذا كان سيتم استبدال خط الحرف فقط عندما لا يكون خط الخلية متوافقًا معه. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق من الصحة قبل حفظ الملف. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | إذا كانت OnePagePerSheet صحيحة ، فسيتم إخراج كل محتويات ورقة واحدة إلى صفحة واحدة فقط نتيجة لذلك. سيكون حجم الورق الخاص بإعداد الصفحات غير صالح ، وستظل الإعدادات الأخرى لإعداد الصفحات سارية المفعول . |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | الحصول على نوع تحسين pdf وتعيينه. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | يشير إلى ما إذا كان سيتم إخراج صفحة فارغة في حالة عدم وجود شيء يمكن طباعته. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | الحصول على أو تحديد عدد الصفحات المراد حفظها. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | الحصول على أو تعيين فهرس للصفحة الأولى على أساس 0 للحفظ. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | التحكم / الإشارة إلى تقدم عملية حفظ الصفحة. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | الإشارة إلى خوارزمية الضغط |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | يشير إلى الصفحات التي لن تتم طباعتها . |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | الحصول على وتعيين منتج مستند pdf الذي تم إنشاؤه. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | يشير إلى ما إذا كان تحديث بيانات ذاكرة التخزين المؤقت للرسم البياني |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | يحصل على تنسيق ملف الحفظ. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | عيّن هذه الخيارات ، عند الحاجة إلى الأمان في نتيجة xls2pdf. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | الحصول على عرض نوع النص أو تعيينه عندما يكون عرض النص أكبر من عرض الخلية. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | يشير إلى ما إذا كان تحديث إعداد الرسم الذكي . القيمة الافتراضية هي false . |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | يشير إلى ما إذا كان يجب التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | الحصول على رد اتصال التحذير أو تعيينه . |

## طُرق

| اسم | وصف |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | يضبط PPI المطلوب (بكسل لكل بوصة) للصور المعاد تشكيلها وجودة jpeg. سيتم تحويل جميع الصور إلى JPEG بإعداد الجودة المحدد ، وستتم إعادة تشكيل الصور الأكبر من PPI المحدد (بكسل لكل بوصة). |

### أنظر أيضا

* class [SaveOptions](../saveoptions)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
