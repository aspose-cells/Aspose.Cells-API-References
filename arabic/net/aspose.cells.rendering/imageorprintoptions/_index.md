---
title: "الفئة ImageOrPrintOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.ImageOrPrintOptions. تسمح بتحديد الخيارات عند تحويل ورقة العمل إلى صور أو طباعة ورقة العمل أو تحويل المخطط إلى صورة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

يسمح بتحديد الخيارات عند تصيير ورقة العمل إلى صور، طباعة ورقة العمل أو تصيير المخطط إلى صورة.

```csharp
public class ImageOrPrintOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | منشئ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) تحديد نوع صورة المخطط عند التحويل. القيمة الافتراضية: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط هذا على true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | يمكن للعميل إخراج خاص إلى الطابعة عند طباعة كل صفحة باستخدام هذا EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | يمكن للعميل التحكم في إعدادات صفحة الطابعة عند طباعة كل صفحة باستخدام هذا EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | يحصل أو يضبط الإعدادات المخصصة أثناء التصيير. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | يحصل أو يضبط لغة التحرير الافتراضية. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | تنفذ هذه الواجهة للحصول على DrawObject و Bound أثناء التصيير. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) تحديد اسم الملف للصورة المضمنة في svg. يجب أن يكون مسارًا كاملاً مع الدليل مثل "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | إعداد لتصوير ملفات Emf الميتا في الملف المصدر. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | يحصل أو يضبط EmfType الذي يحدد تنسيق ملف الميتا. القيمة الافتراضية هي EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | يحصل أو يضبط gridline colr. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | يحصل أو يضبط نوع خطوط الشبكة. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | يحصل أو يضبط الدقة الأفقية للصور المولدة، بوحدة النقاط في البوصة. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | يحصل أو يضبط تنسيق الصور المُولدة. القيمة الافتراضية: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان عرض وارتفاع الخلايا يتم ضبطه تلقائيًا وفقًا لقيمة الخلية. القيمة الافتراضية هي false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | يحدد ما إذا كان سيتم تحسين عناصر الإخراج. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في pagesetup غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يؤثر أي مقياس. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | يحصل أو يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | التحكم/الإشارة إلى تقدم عملية حفظ الصفحة. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | يحصل أو يضبط تنسيق البكسل للصور المولدة. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | يشير إلى الصفحات التي لن تُطبع. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | يحصل أو يضبط قيمة تحدد جودة الصور المولدة لتُطبق فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) يحصل أو يضبط نوع تنسيق ملف الإخراج. يدعم Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | يحصل أو يضبط الأوراق المراد عرضها. القيمة الافتراضية هي جميع الأوراق المرئية في المصنف: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | يحدد ما إذا كان يتم تطبيق التنعيم (إزالة التعرجات) على الخطوط والمنحنيات وحواف المناطق المملوءة. القيمة الافتراضية هي SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) يحصل ويضبط بادئة اسم الـ css في svg، القيمة الافتراضية هي سلسلة فارغة. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) إذا كانت هذه الخاصية true، فإن الـ svg المُولد سيتناسب مع منطقة العرض. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | يحصل أو يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | يحدد جودة عرض النص. القيمة الافتراضية هي TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | يحصل أو يضبط الطريقة المستخدمة أثناء تحويل الصور إلى صيغة 1 bpp عندما يكون [`ImageType`](./imagetype/) هو Tiff و[`TiffCompression`](./tiffcompression/) يساوي Ccitt3 أو Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | يحصل أو يضبط عمق البت لتطبيقه فقط عند حفظ الصفحات بصيغة `Tiff`. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | يحصل أو يضبط نوع الضغط لتطبيقه فقط عند حفظ الصفحات بصيغة `Tiff`. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | يشير إلى ما إذا كان خلفية الصورة المولدة يجب أن تكون شفافة. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | يحصل أو يضبط الدقة العمودية للصور المولدة، بوحدة النقاط في البوصة. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء التحذيري. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) يضبط العرض والارتفاع المطلوبين للصورة. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | يضبط العرض والارتفاع المطلوبين للصورة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // إنشاء ImageOrPrintOptions وضبط الخصائص
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // إنشاء مصنف جديد مع بيانات نموذجية ومخطط
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حفظ المخطط كصورة باستخدام الخيارات
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


