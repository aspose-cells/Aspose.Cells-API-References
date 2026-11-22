---
title: "SparklineGroup.ShowLastPoint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تشير إلى ما إذا كان يجب تمييز آخر نقطة من البيانات في مجموعة sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/showlastpoint/
---
## SparklineGroup.ShowLastPoint property

يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة من البيانات في مجموعة sparkline.

```csharp
public bool ShowLastPoint { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowLastPointDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
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

            // إضافة سباركلين
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // تكوين مظهر السباركلين
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;
            group.LineWeight = 1.0;

            // تمكين وتلوين النقطة الأخيرة
            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            // احفظ المصنف
            workbook.Save("SparklineShowLastPointDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


