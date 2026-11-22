---
title: "الفئة EbookLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.EbookLoadOptions. تمثل الخيارات عند استيراد ملف كتاب إلكتروني"
type: docs
url: /ar/net/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class

يمثل خيارات عند استيراد ملف كتاب إلكتروني.

```csharp
public class EbookLoadOptions : HtmlLoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [EbookLoadOptions](ebookloadoptions/#constructor)() | ينشئ خيارًا لتحميل ملف الكتاب الإلكتروني. |
| [EbookLoadOptions](ebookloadoptions/#constructor_1)(LoadFormat) | ينشئ خيارًا لتحميل ملف الكتاب الإلكتروني. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) الدليل الذي سيتم حفظ الملفات المرفقة فيه.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم الترشيح التلقائي للبيانات عند تحميل الملفات.(موروث من [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | يشير إلى ما إذا كان سيتم ضبط الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | يحصل ويضبط خيارات الملاءمة التلقائية(موروث من [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب(موروث من [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة النص التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف excel، يجب ألا تحفظ المصنف بتنسيق excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف excel المُولد.(موروث من [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. القيمة الافتراضية هي true.(موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) إذا كان true، يتم تحويل السلسلة إلى صيغة عندما يبدأ قيمة السلسلة بالحرف '=', والقيمة الافتراضية هي false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات عددية. القيمة الافتراضية هي true.(موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله(موروث من [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط المصنف(موروث من [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | يشير إلى ما إذا كان سيتم حذف المسافات الزائدة عندما يلتف النص إلى أسطر باستخدام الوسم `<br>`. القيمة الافتراضية هي false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | يشير إلى ما إذا كان سيتم اكتشاف صيغة LaTeX في ملف HTML. القيمة الافتراضية هي false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | يحصل على الترميز الافتراضي ويضبطه. ينطبق فقط على ملفات csv. (موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | يحصل ويضبط تكوينات الخط الفردية. يعمل فقط مع الـ [`Workbook`](../workbook/) الذي يستخدم هذا الـ [`LoadOptions`](../loadoptions/) للتحميل(موروث من [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=".(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | يحدد كيفية تحميل الروابط التشعبية عند تحميل HTML.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرة(موروث من [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة(موروث من [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | يحصل ويضبط مراقب المقاطعة(موروث من [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | يشير إلى ما إذا كان لا يتم تحليل قيمة سلسلة إذا كان طولها 15. (موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true(موروث من [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | يحصل أو يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف(موروث من [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | المرشح لتحديد طريقة تحميل البيانات(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | يحصل على تنسيق التحميل(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | يشير إلى ما إذا كان سيتم استيراد الصيغ إذا كان ملف HTML الأصلي يحتوي على صيغ (Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | يشير إلى الاستراتيجية لتطبيق النمط على القيم المحللة عند تحويل قيمة سلسلة إلى رقم أو تاريخ/وقت. (موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | يحصل أو يضبط وضع الذاكرة للمصنف المحمّل(موروث من [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) يحدد كيفية عرض عناصر HTML &lt;p&gt; عند تحميل HTML. القيمة الافتراضية هي Normal.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | يحدد كيفية عرض عناصر HTML &lt;p&gt; عند تحميل HTML. القيمة الافتراضية هي Normal.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف(موروث من [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false(موروث من [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | يحصل ويضبط كلمة مرور المصنف(موروث من [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي يتم تعبئتها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.(موروث من [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | يحصل على معرف البرنامج لإنشاء الملف. فقط لملفات MHT.(موروث من [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله(موروث من [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) يحدد اسم الخط القياسي الافتراضي(موروث من [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) يحدد حجم الخط القياسي الافتراضي.(موروث من [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | يحصل أو يضبط StreamProviderImportHtmlFile لاستيراد الكائنات.(موروث من [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | يشير إلى ما إذا كان يدعم تخطيط وسم `<div>` عندما يحتوي ملف HTML عليه. القيمة الافتراضية هي false.(موروث من [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | احصل على مثيل HtmlTableLoadOptionCollection(موروث من [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | يحصل على رد الاتصال التحذيري أو يضبطه.(موروث من [`LoadOptions`](../loadoptions/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | يحدد حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية.(موروث من [`LoadOptions`](../loadoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;
    using System.Text;

    public class EbookLoadOptionsDemo
    {
        public static void EbookLoadOptionsExample()
        {
            // إنشاء مثيل من EbookLoadOptions
            EbookLoadOptions options = new EbookLoadOptions();

            // ضبط الخصائص
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // تحميل ملف ebook إلى Workbook باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../htmlloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


