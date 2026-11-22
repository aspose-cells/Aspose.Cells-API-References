---
title: "SlicerCache.List"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SlicerCache. تشير إلى ما إذا كان المقسم المرتبط بذاكرة التخزين المؤقت للمقسم المحدد يعتمد على مصدر بيانات NonOLAP"
type: docs
url: /ar/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

يشير إلى ما إذا كانت أداة التقطيع المرتبطة بذاكرة التخزين المؤقت لأداة التقطيع المحددة تعتمد على مصدر بيانات غير OLAP.

```csharp
public bool List { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyListDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // إنشاء جدول مع التحميل الزائد الصحيح
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // إضافة مقطع
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // الوصول إلى ذاكرة التخزين المؤقت للمقسم
            SlicerCache cache = slicer.SlicerCache;

            // عرض استخدام خاصية List
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### انظر أيضًا

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


