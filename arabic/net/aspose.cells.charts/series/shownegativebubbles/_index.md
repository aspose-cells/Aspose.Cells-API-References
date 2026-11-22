---
title: "Series.ShowNegativeBubbles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية السلسلة. صحيحة إذا تم عرض الفقاعات السالبة لمجموعة المخطط. صالحة فقط لمخططات الفقاعات"
type: docs
url: /ar/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

صحيح إذا تم عرض الفقاعات السلبية لمجموعة المخطط. صالح فقط لمخططات الفقاعات.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لمخطط الفقاعات
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // إضافة مخطط فقاعات
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // الوصول إلى السلسلة الأولى وتعيين خاصية ShowNegativeBubbles
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


