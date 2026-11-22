---
title: "Axis.DisplayUnitLabel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل تسمية وحدة على محور في المخطط المحدد. تسميات الوحدات مفيدة لتصوير القيم الكبيرة مثل الملايين أو المليارات"
type: docs
url: /ar/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

يمثل تسمية وحدة على محور في المخطط المحدد. تسميات الوحدات مفيدة لتصوير القيم الكبيرة - على سبيل المثال، بالملايين أو المليارات.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A1:A4", true);
            
            // قم بتكوين وحدة العرض والتسمية
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // أخرج نص تسمية وحدة العرض
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // احفظ المصنف
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


