---
title: "الفئة PclSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.PclSaveOptions. تمثل الخيارات لحفظ ملف Pcl"
type: docs
url: /ar/net/aspose.cells/pclsaveoptions/
---
## PclSaveOptions class

يمثل خيارات حفظ ملف Pcl.

```csharp
public class PclSaveOptions : PaginatedSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PclSaveOptions](pclsaveoptions/)() | ينشئ الخيارات لحفظ ملف pcl. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | إذا كان AllColumnsInOnePagePerSheet صحيحًا، سيتم إخراج جميع محتويات الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعداد الصفحة، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. (موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
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
| [EmbedFont](../../aspose.cells/pclsaveoptions/embedfont/) { get; set; } | يشير إلى ما إذا كان يجب تضمين الخط في ملف Pcl الناتج. |
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
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | يحصل أو يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.(موروث من [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال التحذيري.(موروث من [`SaveOptions`](../saveoptions/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddPrinterFont](../../aspose.cells/pclsaveoptions/addprinterfont/)(string, string) | يضيف معلومات حول الخط الذي تم إضافته بالفعل إلى الطابعة من قبل الشركة المصنعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassPclSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // إنشاء خيارات حفظ PCL
            PclSaveOptions pclOptions = new PclSaveOptions();
            
            // تكوين خطوط الطابعة (مثال)
            pclOptions.AddPrinterFont("Arial", "ArialPCL");
            pclOptions.AddPrinterFont("Times New Roman", "TimesPCL");
            
            // تعيين خيارات الصفحات الأخرى الموروثة من PaginatedSaveOptions
            pclOptions.OnePagePerSheet = true;
            pclOptions.PageIndex = 0;
            pclOptions.PageCount = 1;
            
            // حفظ المصنف بتنسيق PCL
            workbook.Save("PclSaveOptionsOutput.pcl", pclOptions);
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


