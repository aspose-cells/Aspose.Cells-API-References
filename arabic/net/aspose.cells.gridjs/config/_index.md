---
title: "الفئة Config"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridJs.Config. تمثل جميع الإعدادات الثابتة لـ GridJs."
type: docs
url: /ar/net/aspose.cells.gridjs/config/
---
## Config class

يمثل جميع الإعدادات الثابتة لـ GridJs.

```csharp
public class Config
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Config](config/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | يشير إلى ما إذا كان يجب ضبط عرض الأعمدة تلقائيًا أثناء تحميل الملف. القيمة الافتراضية هي `false`. تحذير: ضبط هذا إلى `true` سيؤدي إلى تنفيذ عملية ضبط تلقائي لجميع الأعمدة بعد التحميل، مما قد يؤثر بشكل ملحوظ على الأداء. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | يشير إلى ما إذا كان يجب ضبط ارتفاع الصفوف تلقائيًا أثناء تحميل الملف. القيمة الافتراضية هي `false`. تحذير: ضبط هذا إلى `true` سيؤدي إلى تنفيذ عملية ضبط تلقائي لجميع الصفوف بعد التحميل، مما قد يؤثر بشكل ملحوظ على الأداء. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | الحصول على/تعيين ما إذا كان يجب تحسين أداء التحميل تلقائيًا لورقة العمل التي تحتوي على خلايا كبيرة. سيتجاهل بعض الأنماط/الحدود لتقليل وقت التحميل. القيمة الافتراضية هي true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | يحصل/يضبط اسم المسار الأساسي لعنوان URL لمتحكم GridJs. القيمة الافتراضية هي "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | الحصول على/تعيين خيارات PdfSaveOptions المخصصة لتصدير PDF. إذا تم تعيينها، سيتم استخدامها بدلاً من الخيارات الافتراضية. القيمة الافتراضية هي null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | الحصول على/تعيين الحد الأقصى الافتراضي للأعمدة لورقة عمل فارغة. القيمة الافتراضية هي 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | الحصول على/تعيين الحد الأقصى الافتراضي للصفوف لورقة عمل فارغة. القيمة الافتراضية هي 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تمكين رسم المخططات من جانب العميل. إذا تم ضبطه على false، سيعود GridJs إلى استخدام صور/أشكال المخططات التي يولدها الخادم فقط. القيمة الافتراضية هي true. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | يحصل/يضبط دليل التخزين المؤقت لتخزين ملف جدول البيانات. نحتاج إلى تعيينه إلى مسار محدد قبل استخدام GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | يحصل/يضبط ما إذا كان سيتم إظهار النطاق الأقصى الذي يشمل البيانات، النمط، الخلايا المدمجة والأشكال. إذا كان الصف أو العمود الأخير يحتوي على خلايا بدون قيمة أو صيغة ولكن لها نمط مخصص، فلن نعرض هذا الصف/العمود عندما تكون هذه القيمة true. القيمة الافتراضية هي true. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | يحصل/يضبط ما إذا كان سيتم دعم التحرير التعاوني، القيمة الافتراضية هي false. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تقييد العدد الإجمالي للأشكال/الصور المعروضة في ورقة عمل واحدة، إذا تم تعيينه إلى true، سيقوم GridJs بتقييد العدد الإجمالي للأشكال أو الصور المعروضة في ورقة عمل واحدة إلى MaxShapeOrImageCount. القيمة الافتراضية هي true. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | يحصل/يضبط ما إذا كان GridJs يعمل داخل مضيف WebAssembly للمتصفح بدلاً من عملية خادم. عندما يكون true، لا يتم استخدام مسار FileCacheDirectory / القرص / مسار مقاطعة الخيط ويجب أن يأتي ذاكرة التخزين المؤقت للملفات من GridJsOptions.CacheImp. تقوم GridJsOptions.IsWasm بتعيين هذا عند إنشاء خدمة GridJs، لذا فإن ملف Aspose.Cells.GridJs.dll واحد يخدم كلا المضيفين. القيمة الافتراضية هي false. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | يحصل/يضبط خيارات تكوين ذاكرة التخزين المؤقت JSON. يتحكم في سلوك الذاكرة (L1) والقرص (L2) للذاكرة المؤقتة للملف JSON الخاص بكتاب العمل المُنشأ. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تحميل ورقة العمل النشطة فقط، القيمة الافتراضية هي false. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | يحصل/يضبط الحد الأقصى لثواني المهلة عند الحفظ إلى PDF. القيمة الافتراضية هي 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | يحصل/يضبط العدد الإجمالي للأشكال أو الصور المعروضة في الورقة النشطة، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | يحصل/يضبط الحد الأقصى للعرض أو الارتفاع لشكل أو صورة، سيتجاهل GridJs الشكل أو الصورة التي يكون عرضها أو ارتفاعها أكبر من ذلك، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | يحصل/يضبط العدد الإجمالي للأشكال أو الصور المعروضة في دفتر العمل، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | يحصل/يضبط وجهات WebSocket التي تبدأ بـ \"/topic\". القيمة الافتراضية هي \"/topic/opr\". تُستخدم في وضع التعاون فقط. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | يحصل/يضبط دليل التخزين المؤقت للصور. (يُطبق هذا عندما يكون GridJsWorkbook.CacheImp فارغًا) سيكون المسار الافتراضي \"_piccache\" داخل FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | يحصل/يضبط ما إذا كان سيتم التحقق مما إذا كانت الصور لها نفس المصدر، القيمة الافتراضية هي true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | يحصل/يضبط ما إذا كان سيتم حفظ ملف HTML كأرشيف zip، القيمة الافتراضية هي false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | يحصل/يضبط ما إذا كان سيتم إظهار ورقة عمل المخطط. القيمة الافتراضية هي false. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | يحصل/يضبط ما إذا كان سيتم تخطي الأشكال غير المرئية لواجهة المستخدم، القيمة الافتراضية هي true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | يحصل/يضبط ما إذا كان سيتم استخدام PageSetup.PrintArea لنطاق العرض في واجهة المستخدم عندما تحتوي ورقة العمل على إعداد PageSetup لـ PrintArea. القيمة الافتراضية هي false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | يعيّن مجلد الخطوط |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | يضبط مجلدات الخطوط |

## الحقول

| الاسم | الوصف |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | يشير إلى ما إذا كان سيتم استخدام معرف مولد من العميل بدلاً من معرف الشكل الفعلي في عمليات التمويه ذات الصلة. |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


