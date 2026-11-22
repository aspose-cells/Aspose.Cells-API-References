---
title: "Axis.IsDisplayUnitLabelShown"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل ما إذا كانت تسمية وحدة العرض معروضة على المحور المحدد"
type: docs
url: /ar/net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

يمثل ما إذا كانت تسمية وحدة العرض تُظهر على المحور المحدد.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### ملاحظات

القيمة الافتراضية هي True. تعمل فقط عندما لا تكون [`DisplayUnit`](../displayunit/) None.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsDisplayUnitLabelShownDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // بيانات عينة
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // قم بتكوين وحدة العرض وإظهار التسمية
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            workbook.Save("AxisPropertyIsDisplayUnitLabelShownDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


