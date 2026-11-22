---
title: "الفئة GridPdfSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridDesktop.Data.GridPdfSaveOptions الفئة. يمثل الخيارات لحفظ ملف pdf"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/
---
## GridPdfSaveOptions class

يمثل خيارات حفظ ملف pdf.

```csharp
public class GridPdfSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridPdfSaveOptions](gridpdfsaveoptions/)() | بناء GridSaveOptions |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CachedFileFolder](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cachedfilefolder/) { get; set; } | مجلد الملفات المؤقت يُستخدم لتخزين بعض البيانات الكبيرة. |
| [CalculateFormula](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/calculateformula/) { get; set; } | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF. |
| [ClearData](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cleardata/) { get; set; } | اجعل المصنف فارغًا بعد حفظ الملف. |
| [Compliance](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/compliance/) { get; set; } | تحويل المصنف إلى pdf سيتم وفقًا لـ PdfCompliance في هذه الخاصية. |
| [CreateDirectory](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdirectory/) { get; set; } | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [CreatedTime](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdtime/) { get; set; } | يحصل على ويضبط وقت إنشاء مستند PDF. |
| [CustomPropertiesExport](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/custompropertiesexport/) { get; set; } | يحصل أو يعيّن قيمة تحدد الطريقة التي يتم تصديرها إلى ملف PDF. القيمة الافتراضية هي None. |
| [DisplayDocTitle](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/displaydoctitle/) { get; set; } | يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند. |
| [EmbedStandardWindowsFonts](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True لتضمين خطوط True type fonts. يؤثر فقط على أحرف ASCII 32-127. الخطوط للأكواد التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط يتم تضمينها دائمًا لمعيار PDF/A-1a و PDF/A-1b. القيمة الافتراضية هي true. |
| [EmfRenderSetting](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/emfrendersetting/) { get; set; } | إعداد لتصوير ملف Emf الميتا. |
| [ExportDocumentStructure](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/exportdocumentstructure/) { get; set; } | يشير إلى ما إذا كان يجب تصدير بنية المستند. |
| [FontEncoding](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/fontencoding/) { get; set; } | يحصل على أو يضبط ترميز الخط المضمن في PDF. |
| [MergeAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان سيتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [OptimizationType](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/optimizationtype/) { get; set; } | يحصل على ويضبط نوع تحسين PDF. |
| [PdfCompression](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/pdfcompression/) { get; set; } | حدد خوارزمية الضغط |
| [Producer](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/producer/) { get; set; } | يحصل على ويضبط المنتج للمستند PDF المُنشأ. |
| [RefreshChartCache](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يتم تحديث بيانات مخزن الرسوم البيانية المؤقت. |
| [SortExternalNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [SortNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [UpdateSmartArt](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعداد Smart Art. القيمة الافتراضية هي false. |
| [ValidateMergedAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetImageResample](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/)(int, int) | يضبط قيمة PPI (بكسل لكل بوصة) المطلوبة لإعادة تحجيم الصور وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG باستخدام إعداد الجودة المحدد، وستتم إعادة تحجيم الصور التي تتجاوز قيمة PPI المحددة (بكسل لكل بوصة). |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


