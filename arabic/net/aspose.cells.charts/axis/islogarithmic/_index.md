---
title: "Axis.IsLogarithmic"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل ما إذا كان نوع مقياس محور القيم لوغاريتميًا أم لا"
type: docs
url: /ar/net/aspose.cells.charts/axis/islogarithmic/
---
## Axis.IsLogarithmic property

يمثل ما إذا كان نوع مقياس محور القيم لوغاريتميًا أم لا.

```csharp
public bool IsLogarithmic { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsLogarithmicDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(100);
            worksheet.Cells["A4"].PutValue(1000);
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(100);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries[0].Values = "B1:B4";

            // تكوين المحور اللوغاريتمي
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 10;
            chart.CategoryAxis.MinValue = 1;
            chart.CategoryAxis.MaxValue = 10000;

            // احفظ المصنف
            workbook.Save("AxisPropertyIsLogarithmicDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


