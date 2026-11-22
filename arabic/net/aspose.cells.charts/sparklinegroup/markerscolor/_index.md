---
title: "SparklineGroup.MarkersColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تحصل وتعيّن لون النقاط في كل خط sparkline داخل مجموعة sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/markerscolor/
---
## SparklineGroup.MarkersColor property

يحصل على اللون ويضبطه لنقاط كل sparkline خطي في مجموعة sparkline.

```csharp
public CellsColor MarkersColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyMarkersColorDemo
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
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // تكوين مظهر السباركلين
            group.ShowMarkers = true;
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // احفظ المصنف
            workbook.Save("SparklineMarkersColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


