---
title: "LegendEntry.Background"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LegendEntry. تحصل وتضبط وضع عرض الخلفية"
type: docs
url: /ar/net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

يحصل ويضبط وضع عرض الخلفية.

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية LegendEntry.BackgroundMode. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // احصل على أول إدخال للوسيلة الإيضاحية
                LegendEntry legendEntry = chart.Legend.LegendEntries[0];

                // عرض قيمة خاصية Background الحالية
                Console.WriteLine("Current Background value: " + legendEntry.Background);

                // تعيين قيمة جديدة لخاصية Background (نظرًا لأنها ليست للقراءة فقط)
                legendEntry.Background = BackgroundMode.Opaque;
                Console.WriteLine("Background after setting to Opaque: " + legendEntry.Background);

                // تعيين قيمة أخرى لخاصية Background
                legendEntry.Background = BackgroundMode.Transparent;
                Console.WriteLine("Background after setting to Transparent: " + legendEntry.Background);

                // احفظ المصنف
                workbook.Save("LegendEntryBackgroundDemo.xlsx");
                Console.WriteLine("Background property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


