---
title: "الفئة SlicerCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Slicers.SlicerCache. تمثّل الوصف المختصر لذاكرة التخزين المؤقت لأداة التقطيع"
type: docs
url: /ar/net/aspose.cells.slicers/slicercache/
---
## SlicerCache class

يمثل وصفًا ملخصًا لذاكرة التخزين المؤقت للمقطّع.

```csharp
public class SlicerCache
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CrossFilterType](../../aspose.cells.slicers/slicercache/crossfiltertype/) { get; set; } | (**Obsolete.**) يشير إلى كيفية إظهار العناصر التي لا تحتوي على بيانات في أداة التقطيع. |
| [List](../../aspose.cells.slicers/slicercache/list/) { get; } | يشير إلى ما إذا كانت أداة التقطيع المرتبطة بذاكرة التخزين المؤقت لأداة التقطيع المحددة تعتمد على مصدر بيانات غير OLAP. |
| [Name](../../aspose.cells.slicers/slicercache/name/) { get; } | يرجع اسم ذاكرة التخزين المؤقت لأداة التقطيع. |
| [SlicerCacheItems](../../aspose.cells.slicers/slicercache/slicercacheitems/) { get; } | يرجع مجموعة SlicerCacheItem التي تحتوي على مجموعة جميع العناصر في ذاكرة التخزين المؤقت لأداة التقطيع. للقراءة فقط |
| [SourceName](../../aspose.cells.slicers/slicercache/sourcename/) { get; } | يرجع اسم ذاكرة التخزين المؤقت لأداة التقطيع هذه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // إنشاء بيانات نموذجية
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";
            
            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;
            
            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;
            
            // إنشاء جدول محوري
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();
            
            // إضافة أداة تقطيع والحصول على ذاكرة التخزين المؤقت الخاصة بها
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, "E12", "fruit");
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
            
            // عرض استخدام SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Items:");
            foreach (SlicerCacheItem item in slicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            book.Save("out.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


