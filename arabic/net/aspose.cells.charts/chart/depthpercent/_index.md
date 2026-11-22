---
title: "Chart.DepthPercent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تمثل عمق المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط بين 20 و 2000٪"
type: docs
url: /ar/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

يمثل عمق مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 في المئة).

```csharp
public int DepthPercent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDepthPercentDemo
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
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين خاصية DepthPercent (تتحكم في عمق المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط)
            chart.DepthPercent = 150; // 150% depth

            // احفظ المصنف
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


