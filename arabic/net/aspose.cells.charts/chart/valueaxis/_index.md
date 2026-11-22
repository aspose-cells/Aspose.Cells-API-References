---
title: "Chart.ValueAxis"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. يحصل على المحور Y للرسوم البيانية"
type: docs
url: /ar/net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

يحصل على المحور Y للمخطط.

```csharp
public Axis ValueAxis { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyValueAxisDemo
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
            worksheet.Cells["B2"].PutValue(100000000);
            worksheet.Cells["B3"].PutValue(200000000);
            worksheet.Cells["B4"].PutValue(300000000);

            // إضافة مخطط وتعيين نطاق البيانات الخاص به
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تكوين خصائص ValueAxis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.HundredMillions;
            chart.ValueAxis.Title.Text = "Values (in 100 millions)";
            chart.ValueAxis.MajorUnit = 1;

            // احفظ المصنف
            workbook.Save("ChartPropertyValueAxisDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


