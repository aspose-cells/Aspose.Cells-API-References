---
title: "TickLabels.AutoScaleFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. True إذا كان النص داخل الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

صحيح إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True.

```csharp
public bool AutoScaleFont { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // بيانات عينة
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(100000);
            cells["B3"].PutValue(150000);
            cells["B4"].PutValue(90000);

            // إنشاء مخطط
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // تكوين بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // تكوين تسميات المحور باستخدام AutoScaleFont
            chart.CategoryAxis.TickLabels.AutoScaleFont = true;
            chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
            
            // احفظ المصنف
            workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


