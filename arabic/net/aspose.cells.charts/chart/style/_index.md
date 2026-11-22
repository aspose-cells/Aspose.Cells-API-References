---
title: "Chart.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل وتعيّن النمط المدمج"
type: docs
url: /ar/net/aspose.cells.charts/chart/style/
---
## Chart.Style property

يحصل على النمط المدمج ويضبطه.

```csharp
public int Style { get; set; }
```

### ملاحظات

يجب أن تكون بين 1 و 48. إرجاع -1 إذا لم يتم تعيينها.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart1 = worksheet.Charts[chartIndex];
            chart1.NSeries.Add("B2:B4", false);
            chart1.NSeries.CategoryData = "A2:A4";

            // إنشاء مخطط آخر ونسخ النمط من المخطط الأول
            chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 10, 20, 18);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex];
            chart2.NSeries.Add("B2:B4", false);
            chart2.NSeries.CategoryData = "A2:A4";
            
            // عرض استخدام خاصية Style
            chart2.Style = chart1.Style;

            // احفظ المصنف
            workbook.Save("ChartStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


