---
title: "الفئة SlicerCacheItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Slicers.SlicerCacheItem. تمثّل عنصر مصدر بيانات أداة التقطيع"
type: docs
url: /ar/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

يمثل عنصر مصدر بيانات المقطّع.

```csharp
public class SlicerCacheItem
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | يحدد ما إذا كان `SlicerCacheItem` محددًا أم لا. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | يرجع نص التسمية لعنصر أداة التقطيع. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheItemDemo
    {
        public static void Run()
        {
            // تحميل المصنف مع أداة التقطيع
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // الحصول على أول أداة تقطيع في المصنف
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // التنقل عبر عناصر ذاكرة التخزين المؤقت لأداة التقطيع
            Console.WriteLine("Slicer Cache Items:");
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
                Console.WriteLine($"Item {i}: Selected={slicerCacheItem.Selected}, Value={slicerCacheItem.Value}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


