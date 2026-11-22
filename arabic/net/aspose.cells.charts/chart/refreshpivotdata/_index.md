---
title: "Chart.RefreshPivotData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تُحدّث بيانات المخطط من جدول محوري"
type: docs
url: /ar/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

يقوم بتحديث بيانات المخطط من جدول محوري.

```csharp
public void RefreshPivotData()
```

### ملاحظات

سنجمع البيانات من مصدر البيانات المحوري إلى تقرير جدول محوري. تُستخدم هذه الطريقة فقط لجمع جميع البيانات إلى مخطط محوري.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بيانات نموذجية إلى الورقة الأولى
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // إنشاء جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // إضافة مخطط
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات مخطط المحور
            chart.PivotSource = "Pivot!PivotTable1";
            
            // تحديث بيانات المحور في المخطط
            chart.RefreshPivotData();
            
            // احفظ المصنف
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


