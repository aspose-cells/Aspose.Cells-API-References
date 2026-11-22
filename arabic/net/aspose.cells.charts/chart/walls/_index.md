---
title: "Chart.Walls"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تُرجع كائن Walls يمثل جدران مخطط ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

تُرجع كائن `Walls` يمثل جدران مخطط ثلاثي الأبعاد.

```csharp
public Walls Walls { get; }
```

### ملاحظات

هذه الخاصية لا تنطبق على مخططات الفطيرة ثلاثية الأبعاد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // إنشاء مخطط عمودي أسطواني
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تكوين أساسيات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // تكوين خصائص الجدران
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // حفظ النتيجة
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


