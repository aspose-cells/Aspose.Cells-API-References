---
title: "Timeline.TopPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Timeline. تُرجع أو تعيّن الإزاحة العمودية لشكل المخطط الزمني من الصف العلوي بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells.timelines/timeline/toppixel/
---
## Timeline.TopPixel property

تُرجع أو تعيّن الإزاحة العمودية لشكل المخطط الزمني من الصف العلوي، بوحدات البكسل.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية Shape.Top. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyTopPixelDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء بيانات عينة
            cells["A1"].Value = "Date";
            cells["A2"].Value = new DateTime(2023, 1, 1);
            cells["A3"].Value = new DateTime(2023, 2, 1);
            cells["A4"].Value = new DateTime(2023, 3, 1);
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // إضافة PivotTable
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // إضافة Timeline
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];

            // تعيين خصائص Timeline بما في ذلك TopPixel
            timeline.TopPixel = 50;
            timeline.HeightPixel = 100;
            timeline.WidthPixel = 300;

            // احفظ المصنف
            book.Save("TimelineTopPixelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


