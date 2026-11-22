---
title: "ChartTextFrame.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل أو تعين نص عنوان الإطار"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

يحصل أو يحدد نص عنوان الإطار.

```csharp
public virtual string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // تعيين نص عنوان المخطط
            chart.Title.Text = "Sample Chart Title";

            // الوصول إلى نص وسيلة الإيضاح وتعديله
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // احفظ المصنف
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


