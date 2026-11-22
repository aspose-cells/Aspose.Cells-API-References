---
title: "الفئة GridImageOrPrintOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions. يسمح بتحديد الخيارات عند تحويل ورقة العمل إلى صور أو طباعة ورقة العمل أو تحويل المخطط إلى صورة"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

يسمح بتحديد الخيارات عند تصيير ورقة العمل إلى صور، طباعة ورقة العمل أو تصيير المخطط إلى صورة.

```csharp
public class GridImageOrPrintOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | بنية GridImageOrPrintOptions |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط هذا على true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | حدد اسم ملف الصورة المضمنة في svg. يجب أن يكون مسارًا كاملاً مع الدليل مثل "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | يحصل أو يضبط EmfType الذي يحدد تنسيق ملف الميتا. القيمة الافتراضية هي EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | يحصل أو يضبط نوع خطوط الشبكة. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | يحصل أو يعيّن الدقة الأفقية للصور المولدة، بوحدات النقاط في البوصة. يُطبق على طريقة توليد الصور باستثناء صور بصيغة Emf. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | يحصل أو يضبط تنسيق الصور المُولدة. القيمة الافتراضية: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | يحدد ما إذا كان سيتم تحسين عناصر الإخراج. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في pagesetup غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يؤثر أي مقياس. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | يحصل أو يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | يحصل أو يضبط تنسيق البكسل للصور المولدة. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | يشير إلى الصفحات التي لن تُطبع. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | يحصل أو يضبط قيمة تحدد جودة الصور المولدة لتُطبق فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | يحدد ما إذا كان يتم تطبيق التنعيم (إزالة التعرجات) على الخطوط والمنحنيات وحواف المناطق المملوءة. القيمة الافتراضية هي SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | إذا كانت هذه الخاصية true، فإن SVG المُولد سيتناسب مع منطقة العرض. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | يحصل أو يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | يحدد جودة عرض النص. القيمة الافتراضية هي TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | يشير إلى ما إذا كان خلفية الصورة المولدة يجب أن تكون شفافة. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | يحصل أو يعيّن الدقة العمودية للصور المولدة، بوحدات النقاط في البوصة. يُطبق على طريقة توليد الصور باستثناء صورة بصيغة Emf. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | يضبط العرض والارتفاع المطلوبين للصورة. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف. فهارس الأوراق تبدأ من الصفر. |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


