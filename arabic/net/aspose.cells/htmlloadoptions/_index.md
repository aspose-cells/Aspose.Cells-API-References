---
title: "فئة HtmlLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.HtmlLoadOptions class. يمثل الخيارات عند استيراد ملف HTML"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

يمثل الخيارات عند استيراد ملف HTML.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions/#constructor)() | إنشاء خيارات تحميل الملف. |
| [HtmlLoadOptions](htmlloadoptions/#constructor_1)(LoadFormat) | إنشاء خيارات تحميل الملف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) الدليل الذي سيتم حفظ الملفات المرفقة فيه. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم الترشيح التلقائي للبيانات عند تحميل الملفات.(موروث من [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | يشير إلى ما إذا كان سيتم ضبط الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | يحصل ويضبط خيارات الملاءمة التلقائية(موروث من [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب(موروث من [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة النص التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف excel، يجب ألا تحفظ المصنف بتنسيق excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف excel المُولد.(موروث من [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. القيمة الافتراضية هي true.(موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) إذا كان true، حوّل السلسلة إلى صيغة عندما يبدأ قيمة السلسلة بالحرف '=', القيمة الافتراضية هي false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات عددية. القيمة الافتراضية هي true.(موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله(موروث من [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط المصنف(موروث من [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | يشير إلى ما إذا كان يتم حذف المسافات الزائدة عندما يلتف النص إلى أسطر باستخدام الوسم `<br>`. القيمة الافتراضية هي false. |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | يشير إلى ما إذا كان سيتم اكتشاف صيغة LaTeX في ملف HTML. القيمة الافتراضية هي false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | يحصل على الترميز الافتراضي ويضبطه. ينطبق فقط على ملفات csv. (موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | يحصل ويضبط تكوينات الخط الفردية. يعمل فقط مع الـ [`Workbook`](../workbook/) الذي يستخدم هذا الـ [`LoadOptions`](../loadoptions/) للتحميل(موروث من [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | يحدد كيفية تحميل الروابط التشعبية عند تحميل HTML. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرة(موروث من [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة(موروث من [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | يحصل ويضبط مراقب المقاطعة(موروث من [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | يشير إلى ما إذا كان لا يتم تحليل قيمة سلسلة إذا كان طولها 15. (موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true(موروث من [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | يحصل أو يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف(موروث من [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | المرشح لتحديد طريقة تحميل البيانات(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | يحصل على تنسيق التحميل(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | يشير إلى ما إذا كان يتم استيراد الصيغ إذا كان ملف HTML الأصلي يحتوي على صيغ |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | يشير إلى الاستراتيجية لتطبيق النمط على القيم المحللة عند تحويل قيمة سلسلة إلى رقم أو تاريخ/وقت. (موروث من [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | يحصل أو يضبط وضع الذاكرة للمصنف المحمّل(موروث من [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) يحدد كيفية عرض عناصر HTML &lt;p&gt; عند تحميل HTML. القيمة الافتراضية هي Normal. |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | يحدد كيفية عرض عناصر HTML &lt;p&gt; عند تحميل HTML. القيمة الافتراضية هي Normal. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف(موروث من [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false(موروث من [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | يحصل ويضبط كلمة مرور المصنف(موروث من [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي يتم تعبئتها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.(موروث من [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | يحصل على معرف البرنامج لإنشاء الملف. ينطبق فقط على ملفات MHT. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله(موروث من [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) يحدد اسم الخط القياسي الافتراضي(موروث من [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) يحدد حجم الخط القياسي الافتراضي.(موروث من [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | يحصل على أو يضبط الـ StreamProviderImportHtmlFile لاستيراد الكائنات. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | يشير إلى ما إذا كان يدعم تخطيط الوسم `<div>` عندما يحتوي ملف HTML عليه. القيمة الافتراضية هي false. |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | احصل على مثيل HtmlTableLoadOptionCollection |
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

    public class HtmlLoadOptionsDemo
    {
        public static void HtmlLoadOptionsExample()
        {
            // أنشئ مثيلًا من HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            loadOptions.LoadFormulas = true;
            loadOptions.SupportDivTag = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.HasFormula = true;
            loadOptions.Encoding = System.Text.Encoding.UTF8;
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = true;
            loadOptions.KeepPrecision = true;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = true;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = true;

            // حمّل ملف HTML إلى مصنف باستخدام HtmlLoadOptions
            Workbook workbook = new Workbook("HtmlLoadOptionsExample_original.html", loadOptions);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("HtmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


