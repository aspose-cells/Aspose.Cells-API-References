---
title: "Timeline.LeftPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Timeline. تُرجع أو تضبط الإزاحة الأفقية لشكل الخط الزمني من عموده الأيسر بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells.timelines/timeline/leftpixel/
---
## Timeline.LeftPixel property

تُرجع أو تضبط الإزاحة الأفقية لشكل الخط الزمني من عموده الأيسر، بوحدات البكسل.

```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Left. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyLeftPixelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();

            // أضف خطًا زمنيًا واحصل عليه من المجموعة
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // عرض خاصية LeftPixel
            timeline.LeftPixel = 150;
            timeline.TopPixel = 50;
            timeline.WidthPixel = 200;
            timeline.HeightPixel = 80;

            // احفظ دفتر العمل
            workbook.Save("TimelineLeftPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


