---
title: "SlicerCacheItemCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SlicerCacheItemCollection. تحصل على كائن SlicerCacheItem حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.slicers/slicercacheitemcollection/item/
---
## SlicerCacheItemCollection indexer

يحصل على كائن SlicerCacheItem حسب الفهرس.

```csharp
public SlicerCacheItem this[int index] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل وإضافة جدول محوري
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مقطع
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = slicers[slicerIndex];
            
            // الوصول إلى عناصر ذاكرة التخزين المؤقت للمقسم باستخدام خاصية Item
            SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
            if (items.Count > 0)
            {
                SlicerCacheItem item = items[0]; // Demonstrating Item property usage
                Console.WriteLine("First slicer item: " + item.Value);
            }
        }
    }
}
```

### انظر أيضًا

* class [SlicerCacheItem](../../slicercacheitem/)
* class [SlicerCacheItemCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


