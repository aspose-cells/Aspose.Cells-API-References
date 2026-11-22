---
title: "ChartDataTable.Border"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. تُرجع كائن Border يمثل حد الكائن"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

يعيد كائن Border الذي يمثل حد الكائن

```csharp
public Line Border { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBorderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
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

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // إظهار جدول البيانات
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // تكوين خصائص الحد
            Line border = dataTable.Border;
            border.Color = System.Drawing.Color.Blue;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.DashType = MsoLineDashStyle.Solid;
            
            // تكوين رؤية حدود الجدول
            dataTable.HasHorizontalBorder = true;
            dataTable.HasVerticalBorder = true;
            dataTable.HasOutlineBorder = true;

            // احفظ المصنف
            workbook.Save("ChartDataTableBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


