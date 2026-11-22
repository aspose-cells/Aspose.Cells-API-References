---
title: "Chart.Legend"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تحصل على وسيلة إيضاح المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

يحصل على مفتاح المخطط.

```csharp
public Legend Legend { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyLegendDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تخصيص وسيلة الإيضاح
            chart.Legend.IsAutomaticSize = false;
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.Width = 400;
            chart.Legend.Height = 50;
            chart.Legend.Font.Size = 12;
            chart.Legend.Font.IsBold = true;

            // احفظ المصنف
            workbook.Save("ChartLegendDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


