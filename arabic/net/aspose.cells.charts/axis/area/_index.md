---
title: "Axis.Area"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تحصل على المنطقة"
type: docs
url: /ar/net/aspose.cells.charts/axis/area/
---
## Axis.Area property

يحصل على `Area`.

```csharp
public Area Area { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // الوصول إلى خصائص منطقة محور الفئة
            chart.CategoryAxis.Area.BackgroundColor = Color.LightBlue;
            chart.CategoryAxis.Area.ForegroundColor = Color.White;
            chart.CategoryAxis.Area.Formatting = FormattingType.Custom;
            
            // احفظ المصنف
            workbook.Save("AxisPropertyAreaDemo_Output.xlsx");
            
            Console.WriteLine("Category Axis Area Background Color: " + chart.CategoryAxis.Area.BackgroundColor);
        }
    }
}
```

### انظر أيضًا

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


