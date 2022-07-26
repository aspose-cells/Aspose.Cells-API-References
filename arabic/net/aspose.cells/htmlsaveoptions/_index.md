---
title: HtmlSaveOptions
second_title: Aspose.Cells لمرجع .NET API
description: يمثل خيارات حفظ ملف html .
type: docs
weight: 3740
url: /ar/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

يمثل خيارات حفظ ملف html .

```csharp
public class HtmlSaveOptions : SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | ينشئ خيارات لحفظ ملف html . |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | ينشئ خيارات لحفظ ملف htm . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | يشير إلى ما إذا كانت إضافة نص تلميح الأداة عندما يتعذر عرض البيانات بالكامل. القيمة الافتراضية هي false . |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | الدليل الذي سيتم حفظ الملفات المرفقة فيه . فقط للحفظ في دفق html . |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | حدد بادئة عنوان URL للملفات المرفقة مثل الصورة في ملف html . فقط للحفظ في دفق html . |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | يتم استخدام مجلد الملف المخزن مؤقتًا لتخزين بعض البيانات الكبيرة. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | الحصول على بادئة اسم css وتعيينها ، القيمة الافتراضية هي "" . |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | اجعل المصنف فارغًا بعد حفظ الملف. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | إذا كان صحيحًا وكان الدليل غير موجود ، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | حدد اسم الخط الافتراضي لتصدير html ، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا ، إذا كانت هذه الخاصية خالية ، فسيستخدم Aspose.Cells خطًا عالميًا له نفس العائلة مع الخط الأصلي ، القيمة الافتراضية هي خالية. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | يشير إلى أنه إذا تم تعطيل التعليقات الشرطية ذات المستوى الأدنى عند تصدير الملف إلى html ، فإن القيمة الافتراضية هي false . |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | في حالة عدم التعيين ، استخدم Encoding.UTF8 كنوع ترميز افتراضي. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | الإشارة إلى ما إذا كان يستبعد الأنماط غير المستخدمة . بالنسبة لملفات html التي تم إنشاؤها ، يمكن أن يؤدي استبعاد الأنماط غير المستخدمة إلى جعل حجم الملف أصغر دون التأثير على التأثيرات المرئية. لذا فإن القيمة الافتراضية لهذه الخاصية هي true . إذا احتاج المستخدم إلى الاحتفاظ بجميع الأنماط في المصنف من أجل html الذي تم إنشاؤه (مثل السيناريو الذي يحتاجه user لاستعادة المصنف من html الذي تم إنشاؤه لاحقًا) ، يرجى تعيين هذه الخاصية على أنها خطأ . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | يشير إلى ما إذا كان سيتم تصدير المصنف بأكمله إلى ملف html. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | الحصول على أو تعيين منطقة الخلية المصدرة لورقة العمل النشطة الحالية . إذا قمت بتعيين هذه السمة ، فسيتم حذف منطقة الطباعة الخاصة بورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | للإشارة إلى ما إذا كان سيتم تصدير بيانات صف سفلي زائفة. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht file إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | يشير إلى ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف إلى html. القيمة الافتراضية هي false . إذا كنت تريد استيراد المخرجات html إلى excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | تشير إلى قاعدة تصدير بيانات ملف html. القيمة الافتراضية هي All . |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | الإشارة إلى ما إذا كان تصدير خصائص المستند. القيمة الافتراضية صحيحة. إذا كنت تريد استيراد ملف html أو mht إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | يشير إلى ما إذا كان تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى لعمود العرض. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | يشير إلى ما إذا كان يتم تصدير الصيغة عند حفظ الملف إلى html. القيمة الافتراضية هي true . إذا كنت تريد استيراد المخرجات html إلى excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | الإشارة إلى ما إذا كان سيتم تصدير البرامج النصية للإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht file إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | الإشارة إلى ما إذا كان سيتم تصدير خطوط الشبكة أم لا. القيمة الافتراضية هي false . |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | الإشارة إلى تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي "true". |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | يحدد ما إذا كانت الصور سيتم حفظها بتنسيق Base64 بتنسيق HTML أو MHTML أو EPUB. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | يشير إلى ما إذا كان سيتم تصدير رؤوس الصفحات . |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | يشير إلى ما إذا كان سيتم تصدير رؤوس الصفحات . |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي كاذبة. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | يشير إلى ما إذا كان يتم تصدير عناوين الصفوف والأعمدة في الورقة عند الحفظ في ملفات HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | الإشارة إلى ما إذا كان تصدير نمط الحدود المماثل عندما لا تدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | يشير إلى ما إذا كان تصدير علامة التبويب المفردة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false . |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | الإشارة إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي صحيحة. إذا كنت تريد استيراد ملف html أو mht إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | الإشارة إلى ما إذا كان تصدير ورقة العمل css بشكل منفصل أم لا. القيمة الافتراضية هي false . |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | الإشارة إلى ما إذا كان تصدير خصائص ورقة العمل. القيمة الافتراضية صحيحة. إذا كنت تريد استيراد ملف html أو mht إلى Excel ، فيرجى الاحتفاظ بالقيمة الافتراضية. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | الحصول على IFilePathProvider أو تعيينه لتصدير ورقة العمل إلى html بشكل منفصل. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | العمود المخفي (عرض هذا العمود هو 0) في Excel ، قبل حفظ هذا في تنسيق html ، إذا كان HtmlHiddenColDisplayType هو "إزالة" ، فلن يتم إخراج العمود المخفي ، إذا كانت القيمة "مخفية" ، فسيكون العمود تم إخراجها ، لكنها كانت مخفية ، والقيمة الافتراضية هي "مخفية" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | الصف المخفي (ارتفاع هذا الصف هو 0) في Excel ، قبل حفظ هذا في تنسيق html ، إذا كان HtmlHiddenRowDisplayType هو "إزالة" ، فلن يتم إخراج الصف المخفي ، إذا كانت القيمة "مخفية" ، فسيكون الصف تم إخراجها ، لكنها كانت مخفية ، والقيمة الافتراضية هي "مخفية" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | يشير إلى ما إذا كان سيتم عرض سلسلة عبر الخلايا بنفس طريقة MS Excel عند حفظ ملف Excel بتنسيق html . افتراضيًا ، تكون القيمة افتراضية ، لذلك ، بالنسبة للسلاسل عبر الخلايا ، هناك اختلاف بسيط بين html الملفات التي تم إنشاؤها بواسطة Aspose.Cells و MS Excel. لكن الأداء لإنشاء ملفات html كبيرة ، فإن تعيين القيمة على Cross سيكون أسرع عدة مرات من تعيينها على Default أو Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | حدد ما إذا كان يتم تصدير تلك الأشكال غير المرئية |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | احصل على كائن ImageOrPrintOptions قبل export |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | يشير إلى ما إذا كان يتم استخدام وحدة قابلة للتطوير لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true . |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | يشير إلى ما إذا كان يتم تصدير ملفات الصور إلى الدليل المؤقت. فقط للحفظ في دفق html . |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | يشير إلى أنه إذا كان يتم تصدير التعليقات عند حفظ الملف إلى html ، فإن القيمة الافتراضية هي false . |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | الإشارة إلى ما إذا كان سيتم استخدام ارتباط المسار الكامل في sheet00x.htm و filelist.xml و tabstrip.htm. القيمة الافتراضية هي false . |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | للإشارة إلى نوع السمة الهدف في رابط &lt;a&gt; ، القيمة الافتراضية هي HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق من الصحة قبل حفظ الملف. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | يشير إلى ما إذا كان يتم دمج عنصر TD فارغ بشكل قسري عند تصدير الملف إلى html. سيتم تقليل حجم ملف html بشكل ملحوظ بعد تعيين القيمة على "صواب". القيمة الافتراضية هي كاذبة. إذا كنت ترغب في استيراد ملف html إلى Excel أو تصدير خطوط الشبكة الكاملة عند حفظ الملف إلى html ، يرجى الاحتفاظ بالقيمة الافتراضية. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | عنوان صفحة html . فقط للحفظ في دفق html . |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | تحليل علامة html في الخلية ، مثل ، كقيمة خلية ، أو كعلامة html ، الافتراضي هو true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | الإشارة إلى ما إذا كان ملف html أو mht هو تفضيل العرض التقديمي. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض تقديمي أكثر جمالًا ، فيرجى ضبط القيمة على true . |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | يشير إلى ما إذا كان تحديث بيانات ذاكرة التخزين المؤقت للرسم البياني |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | يشير إلى ما إذا كان حفظ html كملف فردي. القيمة الافتراضية هي false . |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | يحصل على تنسيق ملف الحفظ. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | يشير إلى ما إذا كان يتم عرض كل الأوراق عند الحفظ كملف html واحد. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | الحصول على أو تعيين IStreamProvider لتصدير الكائنات. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | الحصول على وتعيين بادئة اسم النوع css مثل tr و col و td وما إلى ذلك ، يتم تضمينها في عنصر الجدول الذي يحتوي على سمة TableCssId المحددة. القيمة الافتراضية هي "" . |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | يشير إلى ما إذا كان تحديث إعداد الرسم الذكي . القيمة الافتراضية هي false . |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | يشير إلى ما إذا كان يجب التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | الحصول على رد اتصال التحذير أو تعيينه . |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | يشير إلى ما إذا كان يتم استخدام وحدة قابلة للقياس لوصف عرض العمود عند تصدير الملف إلى html. القيمة الافتراضية هي false . |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | يشير إلى ما إذا كان يتم تكبير أو تصغير html عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى html ، فإن القيمة الافتراضية هي false . |

### أنظر أيضا

* class [SaveOptions](../saveoptions)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
