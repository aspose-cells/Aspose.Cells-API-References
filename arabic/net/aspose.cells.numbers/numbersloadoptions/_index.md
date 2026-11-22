---
title: "الفئة NumbersLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Numbers.NumbersLoadOptions class. تمثل خيارات تحميل ملفات Apple Numbers"
type: docs
url: /ar/net/aspose.cells.numbers/numbersloadoptions/
---
## NumbersLoadOptions class

يمثل خيارات تحميل ملفات Apple Numbers.

```csharp
public class NumbersLoadOptions : LoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [NumbersLoadOptions](numbersloadoptions/)() | المُنشئ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | يحصل على ويضبط خيارات الضبط التلقائي (موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت هذه الخاصية false، سنقبل قيمة النص التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُولد. (موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة لدفتر العمل الذي سيتم تحميله.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | يحصل على إعدادات النمط الافتراضية لتهيئة أنماط دفتر العمل(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | يحصل ويضبط إعدادات الخط الفردية. يعمل فقط مع [`Workbook`](../../aspose.cells/workbook/) الذي يستخدم هذا [`LoadOptions`](../../aspose.cells/loadoptions/) للتحميل.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرة(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | يشير إلى ما إذا كان سيتم تجاهل الأشكال غير المفيدة.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | يحصل ويضبط مراقب المقاطعة.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | ما إذا كان سيُحفظ البيانات غير المُحللة في الذاكرة لدفتر العمل عند تحميله من ملف القالب. القيمة الافتراضية هي true.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | يحصل أو يضبط لغة واجهة المستخدم لإصدار دفتر العمل بناءً على رمز البلد (CountryCode) الذي حفظ الملف.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | المرشح لتحديد طريقة تحميل البيانات.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | يحصل على تنسيق التحميل.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadTableType](../../aspose.cells.numbers/numbersloadoptions/loadtabletype/) { get; set; } | الحصول على وتعيين نوع تحميل جداول متعددة في ورقة عمل واحدة. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | يحصل أو يضبط وضع الذاكرة لدفتر العمل المحمَّل.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان سيتم تحليل الصيغة عند قراءة الملف.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان سيتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | يحصل ويضبط كلمة مرور دفتر العمل.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان سيُحافظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وضبطها. القيمة الافتراضية هي false.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreserveTableName](../../aspose.cells.numbers/numbersloadoptions/preservetablename/) { get; set; } | يشير إلى ما إذا كان يجب الحفاظ على أسماء الجداول عند الاستيراد من Numbers. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية المستخدمة لدفتر العمل الذي سيتم تحميله.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) يضبط اسم الخط القياسي الافتراضي(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) يضبط حجم الخط القياسي الافتراضي.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء للتحذير.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | يضبط حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية.(موروث من [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;
    using System.Globalization;

    public class NumbersLoadOptionsDemo
    {
        public static void NumbersLoadOptionsExample()
        {
            // إنشاء مثيل من NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // ضبط الخصائص
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                Password = "password123",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = false,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new CustomLightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new CustomWarningCallback(),
                AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true },
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = false
            };

            // تحميل ملف Numbers باستخدام خيارات التحميل المحددة
            Workbook workbook = new Workbook("NumbersLoadOptionsExample_original.numbers", loadOptions);

            // حفظ المصنف بتنسيق XLSX
            workbook.Save("NumbersLoadOptionsExample.xlsx");
        }
    }

    // تنفيذ مخصص لـ LightCellsDataHandler
    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool ProcessCell(Cell cell)
        {
            return true;
        }

        public bool ProcessRow(Row row)
        {
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            return true;
        }

        public bool StartRow(int rowIndex)
        {
            return true;
        }

        public bool StartSheet(Worksheet sheet)
        {
            return true;
        }
    }

    // تنفيذ مخصص لـ IWarningCallback
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


