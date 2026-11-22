---
title: "SparklineGroup.Sparklines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. يحصل على مجموعة كائنات Sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/sparklines/
---
## SparklineGroup.Sparklines property

يحصل على مجموعة كائن [`Sparkline`](../../sparkline/)

```csharp
public SparklineCollection Sparklines { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySparklinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // إنشاء مجموعة sparkline
            CellArea location = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 4, EndColumn = 4 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // إضافة مخطط صغير باستخدام خاصية Sparklines
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // تخصيص مظهر المخطط الصغير
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // احفظ المصنف
            workbook.Save("SparklineDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


