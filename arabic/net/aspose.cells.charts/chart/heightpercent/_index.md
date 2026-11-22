---
title: "Chart.HeightPercent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تُعيد أو تُعيّن ارتفاع المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط بين 5 و 500 بالمئة"
type: docs
url: /ar/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

يعيد أو يعيّن ارتفاع مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 في المئة).

```csharp
public int HeightPercent { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
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

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عيّن خاصية HeightPercent (تتحكم في ارتفاع المخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط)
            chart.HeightPercent = 150; // 150% of chart width

            // احفظ المصنف
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


