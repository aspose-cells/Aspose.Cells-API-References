---
title: "ChartArea.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartArea. تحصل على كائن Font للعنصر ChartArea المحدد"
type: docs
url: /ar/net/aspose.cells.charts/chartarea/font/
---
## ChartArea.Font property

تحصل على كائن `Font` للعنصر ChartArea المحدد.

```csharp
public override Font Font { get; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(4000);
            worksheet.Cells["B5"].PutValue(6000);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // احصل على مساحة المخطط
            ChartArea chartArea = chart.ChartArea;
            
            // تعيين خصائص خط منطقة المخطط
            Aspose.Cells.Font font = chartArea.Font;
            font.Name = "Tahoma";
            font.Size = 10;
            font.Color = Color.Blue;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // احفظ المصنف
            workbook.Save("ChartAreaFontDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


