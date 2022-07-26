---
title: ImageOrPrintOptions
second_title: Aspose.Cells لمرجع .NET API
description: يسمح بتحديد الخيارات عند عرض ورقة العمل على الصور أو طباعة ورقة العمل أو عرض المخطط على الصورة.
type: docs
weight: 5140
url: /ar/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

يسمح بتحديد الخيارات عند عرض ورقة العمل على الصور أو طباعة ورقة العمل أو عرض المخطط على الصورة.

```csharp
public class ImageOrPrintOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | إذا كانت AllColumnsInOnePagePerSheet صحيحة ، فسيتم إخراج كافة محتويات العمود في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق الخاص بإعداد الصفحات غير صالح ، وستظل الإعدادات الأخرى لإعداد الصفحات سارية المفعول . |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ، قد تظهر ككتلة في pdf ، image. اضبط هذا على "true" لمحاولة استخدام الخط الافتراضي للمصنف لإظهار هذه الأحرف أولاً. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | يمكن للعميل إخراج إخراج خاص للطابعة عند طباعة كل صفحة باستخدام EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | يمكن للعميل التحكم في إعداد صفحة الطابعة عند طباعة كل صفحة باستخدام EventHandler |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | الحصول على لغة التحرير الافتراضية أو تعيينها. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ، قد تظهر ككتلة في ملف pdf ، image. قم بتعيين الخط الافتراضي مثل MingLiu أو MS Gothic لإظهار هذه الأحرف . إذا كانت هذه الخاصية هي لم يتم تعيينها ، ستستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار أحرف unicode هذه. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | تنفيذ هذه الواجهة للحصول على DrawObject و Bound عند العرض. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | حدد اسم ملف الصورة المضمنة بتنسيق svg. يجب أن يكون هذا المسار كاملًا بالدليل مثل "c: \\ xpsEmbedded" |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | الحصول على أو تعيين EmfType الذي يحدد تنسيق ملف التعريف .. القيمة الافتراضية هي EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | الحصول على نوع خط الشبكة أو تعيينه. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | الحصول على الدقة الأفقية أو ضبطها للصور التي تم إنشاؤها ، بالنقاط في البوصة . يطبق طريقة إنشاء الصورة باستثناء الصور بتنسيق Emf. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | الحصول على أو تحديد تنسيق الصور التي تم إنشاؤها. القيمة الافتراضية: PNG . |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | يشير إلى ما إذا كان عرض الخلايا وارتفاعها يتناسب تلقائيًا مع قيمة الخلية. القيمة الافتراضية هي false . |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | يشير إلى ما إذا كان سيتم استبدال خط الحرف فقط عندما لا يكون خط الخلية متوافقًا معه. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | يشير إلى ما إذا كان سيتم تحسين عناصر الإخراج. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | إذا كانت OnePagePerSheet صحيحة ، فسيتم إخراج كل محتويات ورقة واحدة إلى صفحة واحدة فقط نتيجة لذلك. سيكون حجم الورق الخاص بإعداد الصفحات غير صالح ، وستظل الإعدادات الأخرى لإعداد الصفحات سارية المفعول . |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | إذا كانت هذه الخاصية صحيحة ، فسيتم إخراج منطقة واحدة ولن يسري أي مقياس. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | يشير إلى ما إذا كان سيتم إخراج صفحة فارغة في حالة عدم وجود شيء يمكن طباعته. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | الحصول على أو تحديد عدد الصفحات المراد حفظها. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | الحصول على أو تعيين فهرس للصفحة الأولى على أساس 0 للحفظ. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | التحكم / الإشارة إلى تقدم عملية حفظ الصفحة. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | الحصول على أو تحديد تنسيق البكسل للصور التي تم إنشاؤها. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | يشير إلى الصفحات التي لن تتم طباعتها . |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | إذا كانت PrintWithStatusDialog = true ، فسيكون هناك مربع حوار يعرض حالة الطباعة الحالية. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | الحصول على أو تعيين قيمة تحدد جودة الصور المُنشأة ليتم تطبيقها فقط عند حفظ الصفحات في`JPEG` صيغة. القيمة الافتراضية هي 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | الحصول على أو تعيين نوع تنسيق ملف الإخراج دعم Tiff / XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | يحدد ما إذا كان التنعيم (منع الحواف) مطبقًا على الخطوط والمنحنيات وحواف المساحات المعبأة. القيمة الافتراضية هي SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | إذا كانت هذه الخاصية صحيحة ، فإن svg الذي تم إنشاؤه سوف يتناسب مع عرض المنفذ. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | الحصول على عرض نوع النص أو تعيينه عندما يكون عرض النص أكبر من عرض الخلية. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | يحدد جودة عرض النص. القيمة الافتراضية هي TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | الحصول على عمق البت أو تعيينه ليتم تطبيقه فقط عند حفظ الصفحات في ملف`شجار` صيغة. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | الحصول على نوع الضغط أو تحديده ليتم تطبيقه فقط عند حفظ الصفحات في ملف`شجار` التنسيق . |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | يشير إلى ما إذا كانت خلفية الصورة التي تم إنشاؤها يجب أن تكون شفافة. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | الحصول على الدقة الرأسية للصور المُنشأة أو تعيينها ، بالنقاط في البوصة . يطبق طريقة إنشاء الصورة باستثناء صورة بتنسيق Emf. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | الحصول على رد اتصال التحذير أو تعيينه . |

## طُرق

| اسم | وصف |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | يضبط العرض والارتفاع المطلوبين للصورة. |

### أمثلة

```csharp

[C#]

// تعيين خيارات الصورة أو الطباعة
ImageOrPrintOptions options = new ImageOrPrintOptions();

// تعيين تنسيق صورة الإخراج
options.ImageType = ImageType.Png;

// تعيين الدقة الأفقية
options.HorizontalResolution = 300;

// تعيين الدقة الرأسية
options.VerticalResolution = 300;

// مثيل المصنف
Workbook book = new Workbook("test.xls");

// حفظ الرسم البياني كصورة باستخدام خيارات ImageOrPrint
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'تعيين خيارات الصورة أو الطباعة
Dim options As New ImageOrPrintOptions()

'قم بتعيين تنسيق صورة الإخراج
options.ImageType = ImageType.Png

'تعيين الدقة الأفقية
options.HorizontalResolution = 300

'ضبط الدقة الرأسية
options.VerticalResolution = 300

'إنشاء المصنف
Dim book As New Workbook("test.xls")

'احفظ المخطط كصورة باستخدام خيارات ImageOrPrint
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
