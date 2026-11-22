---
title: "SparklineGroup.ShowFirstPoint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تشير إلى ما إذا كان يجب تمييز أول نقطة بيانات في مجموعة المخططات الصغيرة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/showfirstpoint/
---
## SparklineGroup.ShowFirstPoint property

يشير إلى ما إذا كان يجب تمييز النقطة الأولى من البيانات في مجموعة sparkline.

```csharp
public bool ShowFirstPoint { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowFirstPointDemo
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

            // تحديد موقع السباركلين
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة سباركلين
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // تكوين مظهر السباركلين
            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            // احفظ المصنف
            workbook.Save("SparklineShowFirstPointDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


