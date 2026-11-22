---
title: "Axis.AxisLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. يحصل على مظهر المحور"
type: docs
url: /ar/net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

يحصل على مظهر محور.

```csharp
public Line AxisLine { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisLineDemo
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

            // الوصول إلى محور القيم
            Axis valueAxis = chart.ValueAxis;

            // تخصيص خصائص خط المحور
            valueAxis.AxisLine.Color = Color.Red;
            valueAxis.AxisLine.Style = LineType.DashDot;
            valueAxis.AxisLine.Weight = WeightType.MediumLine;

            // احفظ المصنف
            workbook.Save("AxisLineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


