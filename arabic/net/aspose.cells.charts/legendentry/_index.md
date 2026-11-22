---
title: "الفئة LegendEntry."
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.LegendEntry. تمثل إدخالًا في وسيلة إيضاح المخطط."
type: docs
url: /ar/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

يمثل مدخلًا في مفتاح المخطط.

```csharp
public class LegendEntry
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | صحيح إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) يحصل ويضبط وضع عرض الخلفية. |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | يحصل ويضبط وضع عرض الخلفية. |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | يحصل على كائن [`Font`](./font/) للإطار المخطط (ChartFrame) المحدد. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | يحصل ويضبط ما إذا كان إدخال الوسيلة محذوفًا. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | يحصل أو يضبط عدم تعبئة النص. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) يحصل على كائن [`Font`](./font/) للعنصر LegendEntry المحدد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B4"
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // الوصول إلى إدخال الأسطورة للسلسلة الأولى
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // ضبط خصائص إدخال الأسطورة
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // الوصول وتعديل الخط لإدخال الأسطورة
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // احفظ المصنف
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


