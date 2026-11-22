---
title: "Line.ThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. يحصل ويضبط لون السمة"
type: docs
url: /ar/net/aspose.cells.drawing/line/themecolor/
---
## Line.ThemeColor property

يحصل على ويضبط لون السمة.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### ملاحظات

إذا لم يكن لون السمة الأمامية لونًا من السمة، سيتم إرجاع NULL.

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyThemeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Series 1");
            sheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 2; i <= 6; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i-1));
                sheet.Cells["B" + i].PutValue(i * 10);
                sheet.Cells["C" + i].PutValue(i * 15);
            }

            // إضافة مخطط خطي
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("B1:C6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // تخصيص مظهر السلسلة باستخدام ThemeColor
            var seriesThemes = new List<ThemeColorType> { 
                ThemeColorType.Accent1, 
                ThemeColorType.Accent2 
            };

            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                chart.NSeries[i].Border.ThemeColor = new ThemeColor(seriesThemes[i], 0.6);
                chart.NSeries[i].Border.Style = LineType.Solid;
                chart.NSeries[i].Border.Weight = WeightType.MediumLine;
            }

            // احفظ المصنف
            workbook.Save("LineChartWithThemeColor.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThemeColor](../../../aspose.cells/themecolor/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


