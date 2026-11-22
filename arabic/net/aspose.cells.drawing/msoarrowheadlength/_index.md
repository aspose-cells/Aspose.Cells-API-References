---
title: "التعداد MsoArrowheadLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.MsoArrowheadLength. يعدد عرض نهاية الخط لحدود الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

يسرد عرض نهاية الخط لحد الشكل.

```csharp
public enum MsoArrowheadLength
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Short | `0` | طول نهاية الخط القصير |
| Medium | `1` | طول نهاية الخط المتوسط |
| Long | `2` | طول نهاية الخط الطويل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // إنشاء شكل خط للمخطط
            Line line = chart.Line;

            // تعيين أطوال رأس السهم
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // إخراج أطوال رأس السهم
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // احفظ المصنف
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


