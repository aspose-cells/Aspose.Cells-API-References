---
title: "Chart.SetChartDataRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة المخطط. تحدد نطاق البيانات لمخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

يحدد نطاق البيانات للمخطط.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| منطقة | String | يحدد القيم التي سيتم رسم سلسلة البيانات منها |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSetChartDataRangeWithStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);
            
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


