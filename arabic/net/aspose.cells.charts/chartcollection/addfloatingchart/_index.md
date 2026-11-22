---
title: "ChartCollection.AddFloatingChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartCollection. تضيف مخططًا إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

يضيف مخططًا إلى المجموعة.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ChartType | نوع المخطط |
| يسار | Int32 | الإزاحة الأفقية (x) إلى الزاوية |
| أعلى | Int32 | الإزاحة العمودية (y) إلى الزاوية |
| العرض | Int32 | عرض المخطط |
| الارتفاع | Int32 | ارتفاع المخطط |

### قيمة الإرجاع

[`Chart`](../../chart/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة مخطط عائم بالأبعاد المحددة
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // إضافة بيانات عينة إلى المخطط
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


