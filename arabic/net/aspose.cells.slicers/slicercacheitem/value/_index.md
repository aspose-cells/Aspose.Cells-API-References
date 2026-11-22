---
title: "SlicerCacheItem.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SlicerCacheItem. إرجاع نص التسمية لعنصر الـ slicer"
type: docs
url: /ar/net/aspose.cells.slicers/slicercacheitem/value/
---
## SlicerCacheItem.Value property

يرجع نص التسمية لعنصر أداة التقطيع.

```csharp
public string Value { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع بيانات عينة
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // إنشاء بيانات عينة لجدول محوري
            ws.Cells["A1"].PutValue("Name");
            ws.Cells["A2"].PutValue("Alex");
            ws.Cells["A3"].PutValue("Sam");
            ws.Cells["A4"].PutValue("Alex");
            ws.Cells["A5"].PutValue("John");
            
            // إنشاء جدول محوري
            int index = ws.PivotTables.Add("A1:A5", "E1", "PivotTable1");
            PivotTable pt = ws.PivotTables[index];
            pt.AddFieldToArea(PivotFieldType.Row, "Name");
            
            // إضافة مقطع
            int slicerIndex = ws.Slicers.Add(pt, "Name", "Slicer1");
            Slicer slicer = ws.Slicers[slicerIndex];
            
            // عرض كيفية استخدام خاصية Value
            Console.WriteLine("All items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            // اختر فقط "Alex"
            Console.WriteLine("\nSelecting only Alex:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = (item.Value == "Alex");
            }
            slicer.Refresh();
            
            // إظهار العناصر المحددة
            Console.WriteLine("\nSelected items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                if (item.Selected)
                {
                    Console.WriteLine(item.Value);
                }
            }
            
            // تحديد جميع العناصر
            Console.WriteLine("\nSelecting all items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = true;
            }
            slicer.Refresh();
        }
    }
}
```

### انظر أيضًا

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


