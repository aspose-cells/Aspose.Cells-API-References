---
title: "Chart.SubTitle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل على العنوان الفرعي للمخطط. ينطبق فقط على ملفات ODS"
type: docs
url: /ar/net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

يحصل على العنوان الفرعي للمخطط. ينطبق فقط على ملفات ODS.

```csharp
public Title SubTitle { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySubTitleDemo
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين العنوان الرئيسي
            chart.Title.Text = "Main Chart Title";

            // تعيين العنوان الفرعي
            chart.SubTitle.Text = "Chart Subtitle";
            chart.SubTitle.Font.Size = 12;
            chart.SubTitle.Font.IsBold = true;

            // احفظ المصنف
            workbook.Save("ChartWithSubtitle.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


