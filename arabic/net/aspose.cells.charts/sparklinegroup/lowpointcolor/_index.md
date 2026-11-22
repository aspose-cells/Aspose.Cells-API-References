---
title: "SparklineGroup.LowPointColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تحصل وتعيّن لون أدنى نقاط البيانات في مجموعة المخططات الصغيرة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/lowpointcolor/
---
## SparklineGroup.LowPointColor property

يحصل على اللون ويضبطه لأدنى نقاط البيانات في مجموعة sparkline.

```csharp
public CellsColor LowPointColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLowPointColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // إنشاء مجموعة sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // إضافة مجموعة مخططات صغيرة باستخدام API الصحيح
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // تخصيص مظهر المخطط الصغير
            group.ShowLowPoint = true;
            group.LowPointColor.Color = Color.Red;

            workbook.Save("SparklineLowPointColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


