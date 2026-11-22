---
title: "TimelineCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TimelineCollection. تحصل على Timeline حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

يحصل على Timeline حسب الفهرس.

```csharp
public Timeline this[int index] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // أنشئ جدول pivot أولاً
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // إضافة timeline إلى ورقة العمل
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // الوصول إلى timeline باستخدام خاصية Item حسب الفهرس
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // عرض استخدام timeline
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### انظر أيضًا

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

يحصل على Timeline حسب اسم Timeline.

```csharp
public Timeline this[string name] { get; }
```

### أمثلة

```csharp

[C#]

//احصل على Timeline حسب اسم Timeline.
Timeline objByName = sheet.Timelines["date"];
```

### انظر أيضًا

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


