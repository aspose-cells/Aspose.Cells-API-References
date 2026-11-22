---
title: "Sparkline.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Sparkline. تحصل على فهرس العمود للـ sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

يحصل على فهرس العمود للـ sparkline.

```csharp
public int Column { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
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
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // إضافة sparkline في العمود 4 وتوضيح خاصية Column
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // عرض خاصية column (للقراءة فقط)
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // لتغيير موضع العمود، نحتاج إلى إزالة وإعادة إضافة الـ sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // احفظ دفتر العمل
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


