---
title: "ChartTextFrame.IsTextWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل أو تعيين قيمة تشير إلى ما إذا كان النص ملتفًا"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/istextwrapped/
---
## ChartTextFrame.IsTextWrapped property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان النص مُلتفًا.

```csharp
public virtual bool IsTextWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q2");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(12000);
            sheet.Cells["B3"].PutValue(15000);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // تعيين عنوان المخطط مع التفاف النص
            chart.Title.Text = "Quarterly Sales Report (2023) - This is a long title that will wrap when IsTextWrapped is true";
            chart.Title.IsTextWrapped = true;
            
            // احفظ دفتر العمل
            workbook.Save("ChartTextWrappingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


