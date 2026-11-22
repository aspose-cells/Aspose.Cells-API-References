---
title: "Chart.ShowDataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. يحصل أو يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات"
type: docs
url: /ar/net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات.

```csharp
public bool ShowDataTable { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowDataTableDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            dataSheet.Cells["B1"].PutValue("Column 1");
            dataSheet.Cells["C1"].PutValue("Column 2");
            dataSheet.Cells["A2"].PutValue("Item 1");
            dataSheet.Cells["A3"].PutValue("Item 2");
            dataSheet.Cells["A4"].PutValue("Item 3");
            
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);
            dataSheet.Cells["C2"].PutValue(15);
            dataSheet.Cells["C3"].PutValue(25);
            dataSheet.Cells["C4"].PutValue(35);

            // أضف ورقة مخطط
            int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartIndex];
            
            // إنشاء مخطط
            chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
            
            // تعيين مصدر البيانات
            chart.NSeries.Add("Sheet1!B2:C4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";
            
            // فعّل عرض جدول البيانات
            chart.ShowDataTable = true;
            
            // احفظ المصنف
            workbook.Save("ChartWithDataTable.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


