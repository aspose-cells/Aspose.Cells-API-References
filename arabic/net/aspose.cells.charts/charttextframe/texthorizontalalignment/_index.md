---
title: "ChartTextFrame.TextHorizontalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل وتعيّن محاذاة النص الأفقية"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

يحصل ويحدد محاذاة النص أفقياً.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextHorizontalAlignmentDemo
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

            // إضافة مخطط وتعيين نطاق البيانات الخاص به
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على عنوان المخطط وتعيّن الخصائص
            Title title = chart.Title;
            title.Text = "Sample Chart Title";
            
            // عرض خاصية TextHorizontalAlignment
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            Console.WriteLine("Title horizontal alignment set to: " + title.TextHorizontalAlignment);

            // احفظ المصنف
            workbook.Save("ChartTextHorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


