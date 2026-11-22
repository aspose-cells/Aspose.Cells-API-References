---
title: "Axis.CustUnit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تحدد قيمة مخصصة لوحدة العرض"
type: docs
url: /ar/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

يحدد قيمة مخصصة لوحدة العرض.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية Axis.CustomUnit. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يناير 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
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
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // إضافة مخطط وتعيين نطاق البيانات الخاص به
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // احصل على محور القيمة
            Axis valueAxis = chart.ValueAxis;

            // عرض قيمة CustUnit الحالية (خاصية مهجورة)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // تعيين قيمة وحدة مخصصة جديدة (1,000,000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // عرض قيمة CustUnit الجديدة
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // حفظ النتيجة
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


