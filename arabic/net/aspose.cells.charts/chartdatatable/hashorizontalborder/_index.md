---
title: "ChartDataTable.HasHorizontalBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. True إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/hashorizontalborder/
---
## ChartDataTable.HasHorizontalBorder property

صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية

```csharp
public bool HasHorizontalBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasHorizontalBorderDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تمكين جدول البيانات
            chart.ShowDataTable = true;
            // الحصول على جدول البيانات عبر خاصية ChartDataTable
            ChartDataTable dataTable = chart.ChartDataTable;

            // عرض خاصية HasHorizontalBorder
            dataTable.HasHorizontalBorder = true;
            Console.WriteLine("DataTable HasHorizontalBorder: " + dataTable.HasHorizontalBorder);

            // احفظ المصنف
            workbook.Save("ChartDataTablePropertyHasHorizontalBorderDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


