---
title: "الفئة AbstractTextLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AbstractTextLoadOptions. خيارات شائعة لتحميل القيم النصية"
type: docs
url: /ar/net/aspose.cells/abstracttextloadoptions/
---
## AbstractTextLoadOptions class

خيارات شائعة لتحميل قيم النص.

```csharp
public class AbstractTextLoadOptions : LoadOptions
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم الترشيح التلقائي للبيانات عند تحميل الملفات.(موروث من [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | يحصل ويضبط خيارات الملاءمة التلقائية(موروث من [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب(موروث من [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K مثلًا عبر Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على Exception. إذا كانت هذه الخاصية false، سنقبل قيمة النص التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف excel، يجب ألا تحفظ المصنف بتنسيق excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف excel المُولد.(موروث من [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات تاريخ. القيمة الافتراضية هي true. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. القيمة الافتراضية هي true. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله(موروث من [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط المصنف(موروث من [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | يحصل ويعيّن الترميز الافتراضي. ينطبق فقط على ملفات csv. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | يحصل ويضبط تكوينات الخط الفردية. يعمل فقط مع الـ [`Workbook`](../workbook/) الذي يستخدم هذا الـ [`LoadOptions`](../loadoptions/) للتحميل(موروث من [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرة(موروث من [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | يشير إلى ما إذا كان يتم تجاهل الأشكال غير المفيدة(موروث من [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | يحصل ويضبط مراقب المقاطعة(موروث من [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | يشير إلى عدم تحليل قيمة النص إذا كان طولها 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true(موروث من [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | يحصل أو يضبط لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف(موروث من [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | المرشح لتحديد طريقة تحميل البيانات(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | يحصل على تنسيق التحميل(موروث من [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | يشير إلى الاستراتيجية لتطبيق النمط على القيم المحللة عند تحويل قيمة النص إلى رقم أو تاريخ/وقت. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | يحصل أو يضبط وضع الذاكرة للمصنف المحمّل(موروث من [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف(موروث من [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false(موروث من [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | يحصل ويضبط كلمة مرور المصنف(موروث من [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان سيتم الحفاظ على تلك المسافات وفواصل الأسطر التي يتم تعبئتها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false.(موروث من [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله(موروث من [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) يحدد اسم الخط القياسي الافتراضي(موروث من [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) يحدد حجم الخط القياسي الافتراضي.(موروث من [`LoadOptions`](../loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | يحصل على رد الاتصال التحذيري أو يضبطه.(موروث من [`LoadOptions`](../loadoptions/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | يحدد حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية.(موروث من [`LoadOptions`](../loadoptions/).) |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.Text;

namespace AsposeCellsExamples
{
    // تنفيذ مخصص لـ AbstractTextLoadOptions
    public class CustomTextLoadOptions : AbstractTextLoadOptions
    {
        public CustomTextLoadOptions()
        {
            // تعيين الترميز الافتراضي إلى UTF8
            this.Encoding = Encoding.UTF8;

            // تعيين LoadStyleStrategy إلى None
            this.LoadStyleStrategy = TxtLoadStyleStrategy.None;

            // تمكين تحويل البيانات الرقمية
            this.ConvertNumericData = true;

            // تمكين تحويل البيانات التاريخية
            this.ConvertDateTimeData = true;

            // الحفاظ على الدقة للسلاسل ذات الطول 15
            this.KeepPrecision = true;
        }
    }

    public class TextLoadOptionsDemo
    {
        public static void RunDemo()
        {
            // إنشاء نسخة من CustomTextLoadOptions
            CustomTextLoadOptions loadOptions = new CustomTextLoadOptions();

            // تحميل ملف CSV باستخدام خيارات التحميل المخصصة
            Workbook workbook = new Workbook("TextLoadOptionsDemo_original.csv", loadOptions);

            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];

            // طباعة قيمة الخلية الأولى
            Console.WriteLine(sheet.Cells["A1"].StringValue);

            // حفظ دفتر العمل إلى ملف جديد
            workbook.Save("TextLoadOptionsDemo.xlsx");
            workbook.Save("TextLoadOptionsDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


