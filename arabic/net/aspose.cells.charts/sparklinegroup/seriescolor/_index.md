---
title: "SparklineGroup.SeriesColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تحصل وتعيّن لون المخططات الصغيرة في مجموعة المخططات الصغيرة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/seriescolor/
---
## SparklineGroup.SeriesColor property

يحصل على اللون ويضبطه للـ sparklines في مجموعة sparkline.

```csharp
public CellsColor SeriesColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySeriesColorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // بيانات عينة
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(8);
            ws.Cells["A3"].PutValue(3);
            
            // إنشاء مجموعة sparkline
            CellArea dataRange = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            CellArea locationRange = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 1, EndColumn = 1 };
            int index = ws.SparklineGroups.Add(SparklineType.Column, "A1:A3", false, locationRange);
            
            // تعيين لون السلسلة
            SparklineGroup group = ws.SparklineGroups[index];
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;
            
            wb.Save("SparklineSeriesColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


