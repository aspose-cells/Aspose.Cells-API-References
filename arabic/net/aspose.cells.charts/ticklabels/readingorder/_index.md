---
title: "TickLabels.ReadingOrder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تمثل ترتيب قراءة النص"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

يمثل ترتيب قراءة النص.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // تعيين ترتيب قراءة تسميات العلامات
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // احفظ المصنف
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


