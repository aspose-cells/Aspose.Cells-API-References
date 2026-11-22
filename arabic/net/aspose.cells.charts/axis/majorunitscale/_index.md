---
title: "Axis.MajorUnitScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل مقياس الوحدة الرئيسية لمحور الفئة"
type: docs
url: /ar/net/aspose.cells.charts/axis/majorunitscale/
---
## Axis.MajorUnitScale property

يمثل مقياس الوحدة الرئيسية لمحور الفئة.

```csharp
public TimeUnit MajorUnitScale { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة للجدول الزمني
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 5, 1));
            worksheet.Cells["B4"].PutValue(30);
            
            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // قم بتكوين محور الفئة كمقياس زمني بوحدة رئيسية كل شهرين
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;
            
            workbook.Save("AxisPropertyMajorUnitScaleDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


