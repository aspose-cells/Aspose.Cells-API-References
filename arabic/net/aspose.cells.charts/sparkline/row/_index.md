---
title: "Sparkline.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Sparkline. تحصل على فهرس الصف للـ sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

يحصل على فهرس الصف للـ sparkline.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
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
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // إضافة sparkline في الصف 0، العمود 4
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // عرض موضع الصف (خاصية للقراءة فقط)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // لتغيير الموضع، نحتاج إلى إزالة وإعادة إنشاء الـ sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // احفظ دفتر العمل
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


