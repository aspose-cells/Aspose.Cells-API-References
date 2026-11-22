---
title: "Axis.Title"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تحصل على عنوان هذا المحور في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/axis/title/
---
## Axis.Title property

يحصل على عنوان هذا المحور في المخطط.

```csharp
public Title Title { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTitleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // تكوين العناوين
            chart.Title.Text = "Sample Chart";
            chart.Title.IsVisible = true;
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            
            // تكوين عناوين المحاور
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.IsVisible = true;
            chart.CategoryAxis.Title.Font.Name = "Arial";
            
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.IsVisible = true;
            chart.ValueAxis.Title.Font.Name = "Arial";
            
            // احفظ المصنف
            workbook.Save("AxisPropertyTitleDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


