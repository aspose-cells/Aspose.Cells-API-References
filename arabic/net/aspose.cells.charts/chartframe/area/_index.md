---
title: "ChartFrame.Area"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل على المنطقة"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

يحصل على `area`.

```csharp
public virtual Area Area { get; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAreaDemo
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

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى منطقة المخطط
            ChartArea chartArea = chart.ChartArea;
            
            // عرض وظيفة خاصية Area
            Area area = chartArea.Area;
            Console.WriteLine("Original Formatting: " + area.Formatting);
            
            // تعديل خصائص المنطقة
            area.Formatting = FormattingType.Custom;
            area.BackgroundColor = Color.LightBlue;
            area.ForegroundColor = Color.DarkBlue;
            area.Transparency = 0.3;
            area.InvertIfNegative = true;

            // احفظ المصنف
            workbook.Save("ChartFramePropertyAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


