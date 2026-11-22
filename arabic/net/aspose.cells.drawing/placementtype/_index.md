---
title: "تعداد PlacementType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.PlacementType enum. يمثل الطريقة التي يتم فيها إرفاق كائن الرسم بالخلايا تحته"
type: docs
url: /ar/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا أسفله.

```csharp
public enum PlacementType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| FreeFloating | `0` | لا تتحرك أو تغير الحجم مع الخلايا. |
| Move | `1` | تحرك لكن لا تغير الحجم مع الخلايا. |
| MoveAndSize | `2` | تحرك وغيّر الحجم مع الخلايا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // حدد نوع التوضع للمخطط
            chart.Placement = PlacementType.MoveAndSize;

            // أخرج نوع التوضع
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // احفظ المصنف
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


