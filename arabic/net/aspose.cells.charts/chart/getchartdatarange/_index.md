---
title: "Chart.GetChartDataRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تحصل على نطاق مصدر البيانات للمخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

يحصل على نطاق مصدر البيانات للمخطط.

```csharp
public string GetChartDataRange()
```

### قيمة الإرجاع

مصدر البيانات.

### ملاحظات

يدعم النطاق فقط. إذا كانت Series.Values و Name و XValues في نطاق متصل، سيتم إرجاع نطاق يحتوي عليها.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodGetChartDataRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C4"].PutValue(60);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
            
            // احصل على نطاق بيانات المخطط وعرضه
            string dataRange = chart.GetChartDataRange();
            Console.WriteLine("Chart Data Range: " + dataRange);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


