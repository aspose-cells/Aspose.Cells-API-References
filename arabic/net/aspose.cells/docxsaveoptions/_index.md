---
title: "الفئة DocxSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DocxSaveOptions. تمثل خيارات حفظ ملف .docx"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/
---
## DocxSaveOptions class

يمثل خيارات حفظ ملف .docx.

```csharp
public class DocxSaveOptions : PaginatedSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DocxSaveOptions](docxsaveoptions/#constructor)() | يمثل خيارات حفظ ملف .docx. |
| [DocxSaveOptions](docxsaveoptions/#constructor_1)(bool) | يمثل خيارات حفظ ملف .docx. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | إذا كان AllColumnsInOnePagePerSheet صحيحًا، سيتم إخراج جميع محتويات الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعداد الصفحة، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [AsFlatOpc](../../aspose.cells/docxsaveoptions/asflatopc/) { get; set; } | يشير إلى ما إذا كان الحفظ كملف opc مسطح يمكن توليده بواسطة Open XML SDK |
| [AsNormalView](../../aspose.cells/docxsaveoptions/asnormalview/) { get; set; } | تصدير ملف Excel إلى ملف docx كعرض عادي. إذا كانت هذه الخاصية true ، سيتم إخراج منطقة واحدة، ولن يؤثر أي مقياس. القيمة الافتراضية هي false. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K، سيتم قطعها. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | يحدد ما إذا كان يجب فحص توافق الخط لكل حرف في النص. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط هذا على true لمحاولة استخدام الخط الافتراضي للدفتر لعرض هذه الأحرف أولاً. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | الحصول على أو تعيين إعدادات مخصصة أثناء التصيير. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | الحصول على أو تعيين لغة التحرير الافتراضية. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف يونيكود. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | تنفيذ هذه الواجهة للحصول على DrawObject و Bound أثناء التصيير. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedXlsxAsChartDataSource](../../aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/) { get; set; } | يشير إلى ما إذا كان يتم تضمين ملف xlsx كمصدر بيانات للمخطط. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | إعداد لتصيير ملف Emf التعريفي. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. (موروث من [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | الحصول على أو تعيين لون خطوط الشبكة. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | يحصل أو يضبط نوع خطوط الشبكة.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | يشير إلى ما إذا كنت بحاجة لإخفاء الخطأ أثناء العرض. يمكن أن يكون الخطأ في الشكل أو الصورة أو رسم المخطط، إلخ.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | إذا كان OnePagePerSheet صحيحًا، سيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | يحصل أو يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | التحكم/الإشارة إلى تقدم عملية حفظ الصفحات.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | يشير إلى الصفحات التي لن يتم طباعتها.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. (موروث من [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | يحصل أو يضبط سلوكيات العرض الخاصة بـ Excel التي سيتم تطبيقها.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveAsEditableShapes](../../aspose.cells/docxsaveoptions/saveaseditableshapes/) { get; set; } | احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف Word، حتى يمكنك تعديلها في Word. |
| [SaveAsEditableShaps](../../aspose.cells/docxsaveoptions/saveaseditableshaps/) { get; set; } | (**Obsolete.**) احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف Word. يمكنك تعديلها في Word. |
| [SaveElementType](../../aspose.cells/docxsaveoptions/saveelementtype/) { get; set; } | يشير إلى العناصر التي يجب حفظها. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | يحصل أو يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال التحذيري.(موروث من [`SaveOptions`](../saveoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class DocxSaveOptionsDemo
    {
        public static void DocxSaveOptionsExample()
        {
            // افتح ملف Excel
            Workbook workbook = new Workbook("DocxSaveOptions_original.xlsx");

            // أنشئ مثيلاً من DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();

            // ضبط الخصائص
            saveOptions.DefaultFont = "MS Gothic";
            saveOptions.CheckWorkbookDefaultFont = true;
            saveOptions.CheckFontCompatibility = false;
            saveOptions.IsFontSubstitutionCharGranularity = true;
            saveOptions.OnePagePerSheet = true;
            saveOptions.AllColumnsInOnePagePerSheet = false;
            saveOptions.IgnoreError = true;
            saveOptions.OutputBlankPageWhenNothingToPrint = false;
            saveOptions.PageIndex = 0;  // Starting page index (0-based index)
            saveOptions.PageCount = 2;  // Number of pages to be printed
            saveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            saveOptions.GridlineType = GridlineType.Dotted;
            saveOptions.TextCrossType = TextCrossType.CrossKeep;
            saveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            saveOptions.SheetSet = SheetSet.All;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = @"C:\Cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = false;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // احفظ المستند بتنسيق DOCX
            workbook.Save("DocxSaveOptionsExample.docx", saveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


