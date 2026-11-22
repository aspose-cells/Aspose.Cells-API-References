---
title: "LegendEntry.IsTextNoFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LegendEntry. تحصل أو تضبط عدم تعبئة النص"
type: docs
url: /ar/net/aspose.cells.charts/legendentry/istextnofill/
---
## LegendEntry.IsTextNoFill property

يحصل أو يضبط عدم تعبئة النص.

```csharp
public bool IsTextNoFill { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsTextNoFillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // الوصول إلى إدخال الوسيلة الإيضاحية وتعيين IsTextNoFill
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.IsTextNoFill = true; // Text will have no fill
            
            // احفظ المصنف
            workbook.Save("LegendEntryIsTextNoFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


