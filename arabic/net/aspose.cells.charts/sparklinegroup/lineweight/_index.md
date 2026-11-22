---
title: "SparklineGroup.LineWeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. يحصل على ويضبط وزن الخط في كل sparkline خطي داخل مجموعة الـ sparkline بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

يحصل على وزن الخط ويضبطه في كل sparkline خطي في مجموعة sparkline، بوحدة النقاط.

```csharp
public double LineWeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLineWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // بيانات عينة
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // إنشاء مجموعة sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // تعيين خاصية LineWeight
            group.LineWeight = 2.5; // Thicker line weight for visibility

            workbook.Save("SparklineLineWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


