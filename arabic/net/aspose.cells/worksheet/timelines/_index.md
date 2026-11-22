---
title: "Worksheet.Timelines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. احصل على مجموعة المخططات الزمنية في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

احصل على مجموعة Timeline في ورقة العمل

```csharp
public TimelineCollection Timelines { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTimelinesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // أضف عنصر تحكم المخطط الزمني لجدول المحور
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // احفظ المصنف
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


