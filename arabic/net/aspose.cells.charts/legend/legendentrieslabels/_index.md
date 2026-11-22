---
title: "Legend.LegendEntriesLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Legend. تحصل على تسميات عناصر الأسطورة بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/legend/legendentrieslabels/
---
## Legend.LegendEntriesLabels property

يحصل على تسميات عناصر الأسطورة بعد استدعاء طريقة Chart.Calculate().

```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة Legend.GetLegendLabels. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPropertyLegendEntriesLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان إنشاء عناصر الأسطورة
            chart.Calculate();

            // احصل على الأسطورة
            Legend legend = chart.Legend;

            // عرض تسميات عناصر الأسطورة (باستخدام الخاصية)
            Console.WriteLine("Legend Entries Labels:");
            foreach (string label in legend.LegendEntriesLabels)
            {
                Console.WriteLine(label);
            }

            // احفظ المصنف
            workbook.Save("LegendEntriesLabelsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


