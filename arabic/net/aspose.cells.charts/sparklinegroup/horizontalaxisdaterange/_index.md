---
title: "SparklineGroup.HorizontalAxisDateRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تمثل النطاق الذي يحتوي على قيم التاريخ لبيانات المخطط الصغير"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/
---
## SparklineGroup.HorizontalAxisDateRange property

يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات sparkline.

```csharp
public string HorizontalAxisDateRange { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisDateRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات التاريخ والقيمة للمخطط الصغير
            sheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            sheet.Cells["B1"].PutValue(new DateTime(2023, 2, 1));
            sheet.Cells["C1"].PutValue(new DateTime(2023, 3, 1));
            sheet.Cells["D1"].PutValue(new DateTime(2023, 4, 1));
            
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["D2"].PutValue(3);

            // تحديد مساحة الخلية التي سيُوضع فيها المخطط الصغير
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 1,
                EndRow = 1
            };

            // إضافة مجموعة مخططات صغيرة بمحور تاريخ
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A2:D2", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // تعيين نطاق التاريخ للمحور الأفقي
            group.HorizontalAxisDateRange = "A1:D1";
            group.ShowHorizontalAxis = true;

            // احفظ المصنف
            workbook.Save("SparklineWithDateAxis.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


