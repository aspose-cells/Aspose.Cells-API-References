---
title: "SparklineGroup.VerticalAxisMaxValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تمثل نوع القيمة القصوى للمحور العمودي"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/
---
## SparklineGroup.VerticalAxisMaxValueType property

يمثل نوع القيمة القصوى للمحور العمودي.

```csharp
public SparklineAxisMinMaxType VerticalAxisMaxValueType { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueTypeDemo
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

            // إضافة سباركلين
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // تكوين إعدادات المحور العمودي
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // احفظ المصنف
            workbook.Save("SparklineVerticalAxisDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


