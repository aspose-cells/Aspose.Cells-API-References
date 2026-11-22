---
title: "الفئة AutoFitterOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AutoFitterOptions. تمثيل جميع خيارات الضبط التلقائي."
type: docs
url: /ar/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

يمثل جميع خيارات الضبط التلقائي.

```csharp
public class AutoFitterOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) يوضح ما إذا كان يتم ضبط ارتفاع الصف تلقائيًا عندما يتم دمج الخلايا في صف. القيمة الافتراضية هي false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | يحصل ويضبط نوع ضبط ارتفاع الصف تلقائيًا للخلايا المدمجة. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | يحصل ويضبط نوع ضبط النص الملتف تلقائيًا. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | يحصل أو يضبط لغة التحرير الافتراضية. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | يحصل ويضبط الاستراتيجية المُنسقة. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | يوضح ما إذا كان مناسبًا لأغراض العرض. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | يتجاهل الصفوف/الأعمدة المخفية. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | يحصل ويضبط الحد الأقصى لارتفاع الصف (بوحدة النقطة) عند ضبط الصفوف تلقائيًا. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | يوضح ما إذا كان يتم ضبط الصفوف فقط التي ليس ارتفاعها مخصصًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // إنشاء نطاق A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // دمج الخلايا
            range.Merge();

            // إنشاء نسخة من AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // تطبيق ضبط الصفوف تلقائيًا باستخدام الخيارات المحددة
            worksheet.AutoFitRows(options);

            // احفظ المصنف
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


