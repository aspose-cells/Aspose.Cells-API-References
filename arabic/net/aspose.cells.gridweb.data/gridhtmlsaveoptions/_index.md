---
title: GridHtmlSaveOptions
second_title: Aspose.Cells لمرجع .NET API
description: يمثل خيارات حفظ ملف html .
type: docs
weight: 250
url: /ar/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

يمثل خيارات حفظ ملف html .

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | ينشئ خيارات لحفظ ملف html . |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | ينشئ خيارات لحفظ ملف htm . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | الدليل الذي سيتم حفظ الملفات المرفقة فيه . فقط للحفظ في دفق html . |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | حدد بادئة عنوان URL للملفات المرفقة مثل الصورة في ملف html . فقط للحفظ في دفق html . |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | يتم استخدام مجلد الملف المخزن مؤقتًا لتخزين بعض البيانات الكبيرة. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | اجعل المصنف فارغًا بعد حفظ الملف. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | إذا كان صحيحًا وكان الدليل غير موجود ، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | حدد اسم الخط الافتراضي لتصدير html ، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا ، إذا كانت هذه الخاصية خالية ، فسيستخدم Aspose.Cells خطًا عالميًا له نفس العائلة مع الخط الأصلي ، القيمة الافتراضية هي خالية. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | في حالة عدم التعيين ، استخدم Encoding.UTF8 كنوع ترميز افتراضي. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | يشير إلى ما إذا كان سيتم تصدير المصنف بأكمله إلى ملف html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | الحصول على أو تعيين منطقة الخلية المصدرة لورقة العمل النشطة الحالية. إذا قمت بتعيين هذه السمة ، فسيتم حذف منطقة الطباعة الخاصة بورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | الإشارة إلى ما إذا كان سيتم تصدير خطوط الشبكة أم لا. القيمة الافتراضية هي false . |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | يشير إلى ما إذا كان تصدير العناوين عند حفظ الملف إلى html. القيمة الافتراضية هي false . إذا كنت تريد استيراد ملف html إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | الإشارة إلى تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي "true". |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | يحدد ما إذا كانت الصور سيتم حفظها بتنسيق Base64 بتنسيق HTML أو MHTML أو EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي كاذبة. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | يشير إلى ما إذا كان تصدير علامة التبويب المفردة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false . |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | يشير إلى أنه إذا كان يتم تصدير التعليقات عند حفظ الملف إلى html ، فإن القيمة الافتراضية هي false . |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | الإشارة إلى ما إذا كان سيتم استخدام ارتباط المسار الكامل في sheet00x.htm و filelist.xml و tabstrip.htm. القيمة الافتراضية هي false . |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق من الصحة قبل حفظ الملف. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | عنوان صفحة html . فقط للحفظ في دفق html . |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | تحليل علامة html في الخلية ، مثل ، كقيمة خلية ، أو كعلامة html ، الافتراضي هو true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض التقديمي. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض تقديمي أكثر جمالًا ، فيرجى ضبط القيمة على true . |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | يشير إلى ما إذا كان تحديث بيانات ذاكرة التخزين المؤقت للرسم البياني |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | يحصل على تنسيق ملف الحفظ. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | يشير إلى ما إذا كان يجب التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |

### أنظر أيضا

* class [GridSaveOptions](../gridsaveoptions)
* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* المجسم [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
