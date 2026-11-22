---
title: "ChartDataTable.HasOutlineBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خارجية"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/hasoutlineborder/
---
## ChartDataTable.HasOutlineBorder property

صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خارجية

```csharp
public bool HasOutlineBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasOutlineBorderDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // إظهار جدول البيانات والحصول على كائن ChartDataTable
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // عرض خاصية HasOutlineBorder
            dataTable.HasOutlineBorder = true; // Enable outline border
            Console.WriteLine("DataTable HasOutlineBorder: " + dataTable.HasOutlineBorder);

            // احفظ المصنف
            workbook.Save("ChartDataTableHasOutlineBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


