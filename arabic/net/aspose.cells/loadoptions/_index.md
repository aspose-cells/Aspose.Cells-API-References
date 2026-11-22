---
title: "الفئة LoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LoadOptions. تمثل خيارات تحميل الملف"
type: docs
url: /ar/net/aspose.cells/loadoptions/
---
## LoadOptions class

يمثل خيارات تحميل الملف.

```csharp
public class LoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | إنشاء خيارات تحميل الملف. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | إنشاء خيارات تحميل الملف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | يحصل ويضبط خيارات الملاءمة التلقائية |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص المدخلة كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط دفتر العمل |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | يحصل على ويضبط إعدادات الخط الفردية. يعمل فقط مع الـ[`Workbook`](../workbook/) الذي يستخدم هذا `LoadOptions` للتحميل. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | يشير إلى ما إذا كان سيتم تجاهل الأشكال غير المفيدة. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | يحصل على ويضبط مراقب المقاطعة. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | ما إذا كان سيتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عندما يتم تحميله من ملف القالب. القيمة الافتراضية هي true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | يحصل أو يضبط لغة واجهة المستخدم لإصدار Workbook بناءً على رمز البلد (CountryCode) الذي حفظ الملف. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | المرشح لتحديد كيفية تحميل البيانات. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | يحصل على تنسيق التحميل. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | يحصل على أو يضبط وضع الذاكرة لدفتر العمل المحمَّل. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان سيتم تحليل الصيغة عند قراءة الملف. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان سيتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | يحصل على ويضبط كلمة مرور دفتر العمل. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان سيتم الحفاظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وضبطها. القيمة الافتراضية هي false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) يضبط اسم الخط القياسي الافتراضي |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) يضبط حجم الخط القياسي الافتراضي. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء التحذيري. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | يضبط حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // إنشاء مثال من LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // ضبط الخصائص
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // تحميل مصنف باستخدام LoadOptions المحددة
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // تنفيذ عمليات على دفتر العمل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // احفظ المصنف
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


