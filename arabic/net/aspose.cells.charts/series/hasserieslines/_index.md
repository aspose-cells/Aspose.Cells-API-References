---
title: "Series.HasSeriesLines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. صحيحة إذا كان مخطط عمودي مكدس أو مخطط شريطي يحتوي على خطوط السلسلة أو إذا كان مخطط فطيرة داخل فطيرة أو مخطط شريط داخل فطيرة يحتوي على خطوط وصل بين القسمين. ينطبق فقط على المخططات العمودية المكدسة، المخططات الشريطية، مخططات فطيرة داخل فطيرة أو شريط داخل فطيرة"
type: docs
url: /ar/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

صحيح إذا كان مخطط الأعمدة المتكدسة أو مخطط الشريط يحتوي على خطوط السلسلة أو إذا كان مخطط فطيرة داخل فطيرة أو مخطط شريط داخل فطيرة يحتوي على خطوط وصل بين القسمين. ينطبق فقط على مخططات الأعمدة المتكدسة، مخططات الشرائط، مخططات فطيرة داخل فطيرة، أو مخططات شريط داخل فطيرة.

```csharp
public bool HasSeriesLines { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // إضافة مخطط عمودي مكدس
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة بيانات السلسلة
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // الوصول إلى السلسلة الأولى
            Series series = chart.NSeries[0];
            
            // عرض خاصية HasSeriesLines
            series.HasSeriesLines = true; // Enable series lines
            
            // احفظ المصنف
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


