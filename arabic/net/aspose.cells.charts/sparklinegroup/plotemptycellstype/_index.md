---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تشير إلى كيفية رسم الخلايا الفارغة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

يشير إلى كيفية رسم الخلايا الفارغة.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات مع بعض الخلايا الفارغة
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // حدد CellArea للمخطط الخطي.
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // إضافة مجموعة sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // تحديد كيفية رسم الخلايا الفارغة
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // إضافة مخطط صغير إلى المجموعة
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // احفظ المصنف
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


