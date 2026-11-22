---
title: "TickLabels.NumberFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تمثل سلسلة التنسيق لكائن TickLabels"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

تمثّل سلسلة التنسيق لكائن TickLabels.

```csharp
public string NumberFormat { get; set; }
```

### ملاحظات

سلسلة التنسيق هي نفسها إعداد سلسلة تنسيق مخصصة لخلية. على سبيل المثال، "$0".

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A2:A4", true);

            // تعيين تنسيق الرقم لتسميات العلامات على محور القيم
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // احفظ المصنف
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


