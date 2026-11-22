---
title: "Chart.AutoScaling"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. صحيحة إذا قام Microsoft Excel بتقليل حجم مخطط ثلاثي الأبعاد بحيث يكون أقرب في الحجم إلى المخطط الثنائي الأبعاد المكافئ. يجب أن تكون خاصية RightAngleAxes صحيحة"
type: docs
url: /ar/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

صحيح إذا كان Microsoft Excel يقيّم مخططًا ثلاثي الأبعاد بحيث يكون حجمه أقرب إلى المخطط الثنائي الأبعاد المكافئ. يجب أن تكون الخاصية RightAngleAxes صحيحة.

```csharp
public bool AutoScaling { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عرض خاصية AutoScaling
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // احفظ المصنف
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


