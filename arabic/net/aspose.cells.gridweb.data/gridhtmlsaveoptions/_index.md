---
title: "الفئة GridHtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions. تمثل الخيارات لحفظ ملف html."
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

يمثل الخيارات لحفظ ملف HTML.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | ينشئ خيارات لحفظ ملف html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | ينشئ خيارات لحفظ ملف htm. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | حدد بادئة Url للملفات المرفقة مثل الصورة في ملف html. يُستخدم فقط لحفظ تدفق html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | مجلد الملفات المؤقت يُستخدم لتخزين بعض البيانات الكبيرة. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | إذا كان true ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | حدد اسم الخط الافتراضي لتصدير html، سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية null، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | إذا لم يتم تعيينه، استخدم Encoding.UTF8 كنوع الترميز الافتراضي. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | يشير إلى ما إذا كان يتم تصدير دفتر العمل بالكامل إلى ملف html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | يحصل أو يضبط منطقة CellArea المصدرة لورقة العمل النشطة الحالية. إذا قمت بضبط هذه الخاصية، سيتم إهمال منطقة الطباعة لورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | تشير إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | يشير إلى ما إذا كان يتم تصدير العناوين عند حفظ الملف إلى html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | تشير إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | يحدد ما إذا كانت الصور تُحفظ بصيغة Base64 إلى HTML أو MHTML أو EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | تشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | تشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | يشير إلى ما إذا كان سيتم تصدير التعليقات عند حفظ الملف إلى html، القيمة الافتراضية هي false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | يشير إلى ما إذا كان سيتم استخدام رابط المسار الكامل في sheet00x.htm،filelist.xml و tabstrip.htm. القيمة الافتراضية هي false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | عنوان صفحة html. فقط لحفظ إلى تدفق html. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | تحليل علامة html في الخلية، مثل ، كقيمة خلية، أو كعلامة html، القيمة الافتراضية هي true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يتم تحديث بيانات مخزن مؤقت للمخطط (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | يحصل على تنسيق حفظ الملف. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`GridSaveOptions`](../gridsaveoptions/).) |

### انظر أيضًا

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


