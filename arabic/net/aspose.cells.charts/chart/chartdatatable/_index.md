---
title: "Chart.ChartDataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تمثل جدول بيانات المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

يمثل جدول بيانات المخطط.

```csharp
public ChartDataTable ChartDataTable { get; }
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
    public class ChartPropertyChartDataTableDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // تمكين وتخصيص جدول البيانات
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // تعيين خصائص جدول البيانات
            dataTable.ShowLegendKey = true;
            dataTable.HasBorderHorizontal = true;
            dataTable.HasBorderVertical = true;
            dataTable.HasBorderOutline = true;
            dataTable.AutoScaleFont = true;
            dataTable.BackgroundMode = BackgroundMode.Opaque;

            // تخصيص خط جدول البيانات
            dataTable.Font.Name = "Arial";
            dataTable.Font.Size = 10;
            dataTable.Font.Color = Color.Blue;
            dataTable.Font.IsBold = true;

            // تخصيص حدود جدول البيانات
            dataTable.Border.Color = Color.Red;
            dataTable.Border.Style = LineType.Dash;
            dataTable.Border.Weight = WeightType.MediumLine;

            // احفظ المصنف
            workbook.Save("ChartDataTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


