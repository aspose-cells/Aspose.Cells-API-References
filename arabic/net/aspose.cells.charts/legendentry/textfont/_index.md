---
title: "LegendEntry.TextFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LegendEntry. يحصل على كائن Font للعنصر LegendEntry المحدد"
type: docs
url: /ar/net/aspose.cells.charts/legendentry/textfont/
---
## LegendEntry.TextFont property

يحصل على كائن [`Font`](../font/) للعنصر LegendEntry المحدد.

```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام خاصية LegendEntry.Font. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyTextFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(45);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A1:B1";

            // تمكين الأسطورة
            chart.ShowLegend = true;
            Legend legend = chart.Legend;

            // الوصول إلى أول عنصر أسطورة وتعديل خصائص TextFont الخاصة به
            LegendEntry legendEntry = legend.LegendEntries[0];
            Aspose.Cells.Font font = legendEntry.TextFont;
            
            // تعيين خصائص الخط المتنوعة
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // احفظ المصنف
            workbook.Save("LegendEntryTextFontDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


