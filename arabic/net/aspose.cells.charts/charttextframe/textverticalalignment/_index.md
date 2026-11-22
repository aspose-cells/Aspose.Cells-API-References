---
title: "ChartTextFrame.TextVerticalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل أو تعين محاذاة النص العمودية"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/textverticalalignment/
---
## ChartTextFrame.TextVerticalAlignment property

يحصل أو يحدد محاذاة النص عمودياً.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextVerticalAlignmentDemo
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

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // تعيين العنوان وتكوين المحاذاة العمودية
            chart.Title.Text = "Sample Chart";
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // تكوين تسمية وحدة العرض
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.DisplayUnitLabel.Text = "Values in Hundreds";
            chart.ValueAxis.DisplayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;

            // احفظ المصنف
            workbook.Save("ChartTextVerticalAlignmentDemo.xlsx");

            Console.WriteLine("Demo executed successfully. Output file: ChartTextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


