---
title: "Axis.TickLabelSpacing"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل عدد الفئات أو السلاسل بين تسميات علامات الفواصل. ينطبق فقط على محاور الفئة والسلاسل"
type: docs
url: /ar/net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

يمثل عدد الفئات أو السلاسل بين تسميات علامات الفواصل. ينطبق فقط على محاور الفئات والسلاسل.

```csharp
public int TickLabelSpacing { get; set; }
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
    public class AxisPropertyTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // قم بتكوين تباعد تسميات علامات الفواصل للمحور
            chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label

            workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


