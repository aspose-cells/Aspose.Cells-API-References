---
title: "Line.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تمثل لون الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/color/
---
## Line.Color property

يمثل لون الخط.

```csharp
public Color Color { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ضبط ألوان خطوط المحور
            chart.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            chart.ValueAxis.AxisLine.Color = Color.BlueViolet;
            
            // ضبط لون خط عنوان المحور
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.Font.Color = Color.BlueViolet;

            // احفظ المصنف
            workbook.Save("LinePropertyColorDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


