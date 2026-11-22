---
title: "DisplayUnitLabel.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DisplayUnitLabel. يحصل أو يضبط نص تسمية وحدة العرض"
type: docs
url: /ar/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

يحصل أو يضبط نص تسمية وحدة العرض.

```csharp
public override string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A1:A4", true);
            
            // تكوين تسمية وحدة العرض
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // الوصول وتعديل نص تسمية وحدة العرض
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // تغيير النص
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // احفظ المصنف
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


