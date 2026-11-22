---
title: "SparklineGroup.FirstPointColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تحصل وتضبط لون النقطة الأولى للبيانات في مجموعة المخططات الصغيرة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/firstpointcolor/
---
## SparklineGroup.FirstPointColor property

يحصل على اللون ويضبطه للنقطة الأولى من البيانات في مجموعة sparkline.

```csharp
public CellsColor FirstPointColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyFirstPointColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // إنشاء مجموعة sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 1;
            ca.EndColumn = 1;
            
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // تعيين FirstPointColor
            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            // احفظ المصنف
            workbook.Save("SparklineFirstPointColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


