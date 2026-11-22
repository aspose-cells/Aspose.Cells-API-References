---
title: "الفئة GridJsOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridJs.GridJsOptions class. تمثل جميع خيارات التحميل لـ GridJs"
type: docs
url: /ar/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

يمثل جميع خيارات التحميل لـ GridJs

```csharp
public class GridJsOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | يشير إلى ما إذا كان يجب ضبط عرض الأعمدة تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | يشير إلى ما إذا كان يجب ضبط ارتفاع الصفوف تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | الحصول على/تعيين ما إذا كان يجب تحسين أداء التحميل تلقائيًا لورقة العمل التي تحتوي على خلايا كبيرة. سيتجاهل بعض الأنماط/الحدود لتقليل وقت التحميل. القيمة الافتراضية هي true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | الحصول على/تعيين الاسم الأساسي لعنوان URL للمسار الخاص بمتحكم GridJs. القيمة الافتراضية هي GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | الحصول على/تعيين خيارات PdfSaveOptions المخصصة لتصدير PDF. إذا تم تعيينها، سيتم استخدامها بدلاً من الخيارات الافتراضية. القيمة الافتراضية هي null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | الحصول على/تعيين الحد الأقصى الافتراضي للأعمدة لورقة عمل فارغة. القيمة الافتراضية هي 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | الحصول على/تعيين الحد الأقصى الافتراضي للصفوف لورقة عمل فارغة. القيمة الافتراضية هي 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | الحصول على/تعيين ما إذا كان يجب تمكين عرض المخططات من جانب العميل. إذا تم تعيينه إلى false، سيقوم GridJs بإصدار صور/أشكال المخططات فقط ولن يتطلب عرض المخططات من جانب العميل. القيمة الافتراضية هي true. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | يحصل/يضبط دليل التخزين المؤقت لتخزين ملف جدول البيانات. نحتاج إلى تعيينه إلى مسار محدد قبل استخدام GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | يحصل/يضبط مجلدات الخطوط للخطوط في الصور/الأشكال المرسومة |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | يحصل/يضبط ما إذا كان سيتم إظهار النطاق الأقصى الذي يشمل البيانات، النمط، الخلايا المدمجة والأشكال. إذا كان الصف أو العمود الأخير يحتوي على خلايا بدون قيمة أو صيغة ولكن لها نمط مخصص، فلن نعرض هذا الصف/العمود عندما تكون هذه القيمة true. القيمة الافتراضية هي true. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | يحصل/يضبط ما إذا كان سيتم دعم التحرير التعاوني، القيمة الافتراضية هي false. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تقييد العدد الإجمالي للأشكال/الصور المعروضة في ورقة عمل واحدة، إذا تم تعيينه إلى true، سيقوم GridJs بتقييد العدد الإجمالي للأشكال أو الصور المعروضة في ورقة عمل واحدة إلى MaxShapeOrImageCount. القيمة الافتراضية هي true. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | يحصل/يضبط ما إذا كان GridJs يعمل داخل مضيف WebAssembly في المتصفح بدلاً من عملية خادم. عندما تكون القيمة true، لا يتم استخدام FileCacheDirectory / القرص / مسار مقاطعة الخيط، ويجب أن يأتي ذاكرة التخزين المؤقت للملفات من CacheImp، لأن مضيف المتصفح لا يمتلك قرصًا محليًا. يختار مسارات الشيفرة في وقت التشغيل، لذا فإن ملف Aspose.Cells.GridJs.dll واحد يخدم كلا المضيفين. القيمة الافتراضية هي false. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | يحصل/يضبط خيارات تكوين ذاكرة التخزين المؤقت JSON. يتحكم في سلوك الذاكرة (L1) والقرص (L2) للذاكرة المؤقتة للملف JSON الخاص بكتاب العمل المُنشأ. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تحميل ورقة العمل النشطة فقط، القيمة الافتراضية هي false. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | يحصل/يضبط الحد الأقصى لثواني المهلة عند الحفظ إلى PDF. القيمة الافتراضية هي 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | يحصل/يضبط العدد الإجمالي للأشكال أو الصور المعروضة في الورقة النشطة، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | يحصل/يضبط الحد الأقصى للعرض أو الارتفاع لشكل أو صورة، سيتجاهل GridJs الشكل أو الصورة التي يكون عرضها أو ارتفاعها أكبر من ذلك، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | يحصل/يضبط العدد الإجمالي للأشكال أو الصور المعروضة في دفتر العمل، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | يحصل/يضبط وجهات WebSocket التي تبدأ بـ \"/topic\". القيمة الافتراضية هي \"/topic/opr\". تُستخدم في وضع التعاون فقط. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | يحصل/يضبط دليل التخزين المؤقت للصور. (يُطبق هذا عندما يكون GridJsWorkbook.CacheImp فارغًا) سيكون المسار الافتراضي \"_piccache\" داخل FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | يحصل/يضبط ما إذا كان سيتم التحقق مما إذا كانت الصور لها نفس المصدر، القيمة الافتراضية هي true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | يحصل/يضبط ما إذا كان سيتم حفظ ملف HTML كأرشيف zip، القيمة الافتراضية هي false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | يحصل/يضبط ما إذا كان سيتم إظهار ورقة عمل المخطط. القيمة الافتراضية هي false. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تخطي الأشكال غير المرئية لواجهة المستخدم، القيمة الافتراضية هي true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | يحصل/يضبط ما إذا كان سيتم استخدام PageSetup.PrintArea لنطاق العرض في واجهة المستخدم عندما تحتوي ورقة العمل على إعداد PageSetup لـ PrintArea. القيمة الافتراضية هي false. |

## الحقول

| الاسم | الوصف |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | تنفيذ مخصص لتخزين الذاكرة المؤقتة، إذا كنت ترغب في تخزين الذاكرة المؤقتة بطريقة تدفق، تحتاج إلى تعيينه وتنفيذه. يجب على مضيف WebAssembly (IsWasm = true) تعيينه، لأنه لا يوجد قرص محلي لذاكرة التخزين المؤقت الافتراضية. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | يشير إلى ما إذا كان سيتم استخدام معرف مولد من العميل بدلاً من معرف الشكل الفعلي في عمليات التمويه ذات الصلة. |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


