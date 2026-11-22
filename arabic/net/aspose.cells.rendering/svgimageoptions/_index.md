---
title: "الفئة SvgImageOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.SvgImageOptions. خيارات لإنشاء صورة Svg"
type: docs
url: /ar/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

خيارات إنشاء صورة SVG.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | منشئ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | إذا كان AllColumnsInOnePagePerSheet صحيحًا، فسيتم إخراج جميع محتويات الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) تحديد نوع صورة المخطط عند التحويل. القيمة الافتراضية: PNG. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في PDF أو صورة. اضبط هذا على true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | يحصل ويضبط بادئة اسم CSS في SVG، القيمة الافتراضية هي سلسلة فارغة. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | يمكن للعميل إخراج خاص إلى الطابعة عند طباعة كل صفحة باستخدام معالج الحدث هذا (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | يمكن للعميل التحكم في إعدادات صفحة الطابعة عند طباعة كل صفحة باستخدام معالج الحدث هذا (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | يحصل أو يضبط الإعدادات المخصصة أثناء العرض. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | يحصل أو يضبط لغة التحرير الافتراضية. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في PDF أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف يونيكود. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | تنفيذ هذه الواجهة للحصول على DrawObject و Bound عند العرض. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | يحصل أو يضبط نوع الخط المضمن في SVG. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) تحديد اسم ملف الصورة المضمنة في SVG. يجب أن يكون مسارًا كاملاً مع الدليل مثل "c:\\xpsEmbedded" (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | إعداد لعرض ملفات الميتافا Emf في الملف المصدر. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | يحصل أو يضبط EmfType الذي يحدد تنسيق ملف الميتافا. القيمة الافتراضية هي EmfPlusDual. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | إذا كانت هذه الخاصية true، فإن SVG المُولد سيتناسب مع منطقة العرض. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | يحصل أو يضبط لون خطوط الشبكة. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | يحصل أو يضبط نوع خطوط الشبكة. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | يحصل أو يضبط الدقة الأفقية للصور المُولدة، بوحدة النقاط في البوصة. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | يحصل أو يضبط تنسيق الصور المُولدة. القيمة الافتراضية: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان عرض وارتفاع الخلايا يتم ضبطهما تلقائيًا وفقًا لقيمة الخلية. القيمة الافتراضية هي false. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | يحدد ما إذا كان سيتم استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | يحدد ما إذا كان سيتم تحسين عناصر الإخراج. (موروث من [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يؤثر أي مقياس.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | يشير إلى ما إذا كان سيتم إخراج صفحة فارغة عندما لا يوجد شيء للطباعة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | يحصل أو يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | التحكم/الإشارة إلى تقدم عملية حفظ الصفحات.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | يحصل أو يضبط تنسيق البكسل للصور المُولدة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | يشير إلى الصفحات التي لن يتم طباعتها.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | يحصل أو يضبط قيمة تحدد جودة الصور المُولدة لتُطبق فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) يحصل أو يضبط نوع تنسيق ملف الإخراج. يدعم Tiff/XPS.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: [`Visible`](../sheetset/visible/).(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | يحدد ما إذا كان سيتم تطبيق التنعيم (مضاد التعرج) على الخطوط والمنحنيات وحواف المناطق المملوءة. القيمة الافتراضية هي SmoothingMode.None.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) يحصل ويضبط بادئة اسم css في svg، القيمة الافتراضية هي سلسلة فارغة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) إذا كانت هذه الخاصية صحيحة، سيتناسب svg المُولد مع مساحة العرض.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | يحصل أو يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | يحدد جودة عرض النص. القيمة الافتراضية هي TextRenderingHint.SystemDefault.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | يحصل أو يضبط الطريقة المستخدمة أثناء تحويل الصور إلى تنسيق 1 bpp عندما يكون [`ImageType`](../imageorprintoptions/imagetype/) هو Tiff و[`TiffCompression`](../imageorprintoptions/tiffcompression/) يساوي Ccitt3 أو Ccitt4.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | يحصل أو يضبط عمق البت لتطبيقه فقط عند حفظ الصفحات بتنسيق `Tiff`.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | يحصل أو يضبط نوع الضغط لتطبيقه فقط عند حفظ الصفحات بتنسيق `Tiff`.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | يشير إلى ما إذا كان خلفية الصورة المُولدة يجب أن تكون شفافة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | يحصل أو يضبط الدقة العمودية للصور المُولدة، بالنقطة لكل بوصة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء للتحذير.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) يحدد العرض والارتفاع المطلوبين للصورة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | يحدد العرض والارتفاع المطلوبين للصورة.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بيانات عينة للمخطط
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // إنشاء مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // تهيئة خيارات صورة SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // تكوين خيارات عرض SVG
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // تعيين جودة الطباعة والدقة
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // عرض المخطط إلى SVG باستخدام الخيارات المكوَّنة
            chart.ToImage("chart_output.svg", svgOptions);

            // عرض تكامل حفظ المصنف
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


