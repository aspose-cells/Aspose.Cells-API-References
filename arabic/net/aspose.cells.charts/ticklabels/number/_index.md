---
title: "TickLabels.Number"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تمثل رقم التنسيق لكائن TickLabels"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

تمثّل رقم التنسيق لكائن TickLabels.

```csharp
public int Number { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // تكوين تسميات العلامات
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // احفظ المصنف
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


