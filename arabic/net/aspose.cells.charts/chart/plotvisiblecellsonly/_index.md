---
title: "Chart.PlotVisibleCellsOnly"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط"
type: docs
url: /ar/net/aspose.cells.charts/chart/plotvisiblecellsonly/
---
## Chart.PlotVisibleCellsOnly property

يشير إلى ما إذا كان يتم عرض خلايا المخطط المرئية فقط.

```csharp
public bool PlotVisibleCellsOnly { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsOnlyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            
            // إخفاء الصف 3
            worksheet.Cells.Rows[2].IsHidden = true;
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // حدد PlotVisibleCellsOnly إلى false (القيمة الافتراضية هي true)
            chart.PlotVisibleCellsOnly = false;
            
            // احفظ المصنف
            workbook.Save("ChartPlotVisibleCellsOnlyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


