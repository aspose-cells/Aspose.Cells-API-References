---
title: "Series.SizeRepresents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحصل أو تعين ما تمثله حجم الفقاعات في مخطط الفقاعات"
type: docs
url: /ar/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

يحصل على أو يضبط ما تمثله حجم الفقاعة في مخطط الفقاعات.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### ملاحظات

BubbleSizeRepresents.SizeIsArea يعني أن القيمة [`BubbleSizes`](../bubblesizes/) هي مساحة الفقاعة. BubbleSizeRepresents.SizeIsWidth يعني أن القيمة [`BubbleSizes`](../bubblesizes/) هي عرض الفقاعة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لمخطط الفقاعات
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // إضافة مخطط فقاعات
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // تعيين بيانات السلسلة
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // تعيين خاصية SizeRepresents
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // احفظ المصنف
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


