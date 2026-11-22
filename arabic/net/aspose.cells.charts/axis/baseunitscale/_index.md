---
title: "Axis.BaseUnitScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المحور. تمثل مقياس الوحدة الأساسية لمحور الفئة"
type: docs
url: /ar/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

يمثل مقياس الوحدة الأساسية لمحور الفئة.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### ملاحظات

يتم تطبيقه فقط عندما تكون خاصية CategoryType مضبوطة على TimeScale.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // تعيين مقياس الوحدة الأساسية لمحور الفئة
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // احفظ المصنف
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


