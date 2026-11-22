---
title: "ChartDataTable.ShowLegendKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartDataTable. True إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئيًا"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/showlegendkey/
---
## ChartDataTable.ShowLegendKey property

صحيح إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئياً.

```csharp
public bool ShowLegendKey { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyShowLegendKeyDemo
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

            // تمكين جدول البيانات مع مفتاح وسيلة الإيضاح
            chart.ShowDataTable = true;
            // الوصول إلى DataTable عبر خصائص المخطط
            if (chart.ChartDataTable != null)
            {
                chart.ChartDataTable.ShowLegendKey = true;
            }

            // احفظ المصنف
            workbook.Save("ChartDataTableShowLegendKeyDemo.xlsx");

            Console.WriteLine("Chart created with ShowLegendKey enabled in data table.");
        }
    }
}
```

### انظر أيضًا

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


