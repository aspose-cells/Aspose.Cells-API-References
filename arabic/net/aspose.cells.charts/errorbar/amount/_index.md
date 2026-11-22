---
title: "ErrorBar.Amount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ErrorBar. تمثل مقدار شريط الخطأ"
type: docs
url: /ar/net/aspose.cells.charts/errorbar/amount/
---
## ErrorBar.Amount property

يمثل مقدار شريط الخطأ.

```csharp
public double Amount { get; set; }
```

### ملاحظات

يجب أن يكون المبلغ أكبر من أو يساوي الصفر.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyAmountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تكوين أشرطة الخطأ
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5; // Demonstrate Amount property
            }

            workbook.Save("ErrorBarAmountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


