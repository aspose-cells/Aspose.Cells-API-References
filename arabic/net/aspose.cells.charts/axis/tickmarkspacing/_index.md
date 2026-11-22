---
title: "Axis.TickMarkSpacing"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تُرجع أو تضبط عدد الفئات أو السلاسل بين علامات الفواصل. ينطبق فقط على محاور الفئات والسلاسل"
type: docs
url: /ar/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

يرجع أو يعيّن عدد الفئات أو السلاسل بين علامات الفواصل. ينطبق فقط على محاور الفئات والسلاسل.

```csharp
public int TickMarkSpacing { get; set; }
```

### ملاحظات

يجب أن يكون الرقم بين 1 و 31999.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickMarkSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تكوين محور القيم باستخدام TickMarkSpacing
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // تكوين محور الفئات باستخدام TickMarkSpacing
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


