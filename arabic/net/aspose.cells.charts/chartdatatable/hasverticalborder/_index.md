---
title: "ChartDataTable.HasVerticalBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. True إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/hasverticalborder/
---
## ChartDataTable.HasVerticalBorder property

صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية

```csharp
public bool HasVerticalBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasVerticalBorderDemo
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

            // إظهار جدول البيانات
            chart.ShowDataTable = true;
            
            // الوصول إلى جدول البيانات عبر خاصية ChartDataTable
            ChartDataTable dataTable = chart.ChartDataTable;

            // عرض خاصية HasVerticalBorder
            Console.WriteLine("Initial HasVerticalBorder value: " + dataTable.HasVerticalBorder);
            
            // تبديل الحدود العمودية
            dataTable.HasVerticalBorder = true;
            Console.WriteLine("After setting HasVerticalBorder to true: " + dataTable.HasVerticalBorder);
            
            dataTable.HasVerticalBorder = false;
            Console.WriteLine("After setting HasVerticalBorder to false: " + dataTable.HasVerticalBorder);

            // احفظ المصنف
            workbook.Save("ChartDataTable_HasVerticalBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


