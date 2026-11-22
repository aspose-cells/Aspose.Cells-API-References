---
title: "Chart.PivotSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا فإن المخطط هو PivotChart"
type: docs
url: /ar/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا، يكون المخطط PivotChart.

```csharp
public string PivotSource { get; set; }
```

### ملاحظات

إذا كان جدول المحور "PivotTable1" في ورقة العمل "Sheet1" في الملف "Book1.xls". يمكن أن يكون pivotSource هو "[Book1.xls]Sheet1!PivotTable1" إذا لم يكن المخطط و PivotTable في نفس المصنف. إذا قمت بتعيين هذه الخاصية، سيتم فقدان إعداد مصدر البيانات السابق.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر المحور للمخطط
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // تحديث بيانات المحور والمخطط
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // احفظ المصنف
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


