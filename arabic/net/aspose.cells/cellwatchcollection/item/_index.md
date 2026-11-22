---
title: "CellWatchCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellWatchCollection. تحصل وتضبط CellWatch حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/cellwatchcollection/item/
---
## CellWatchCollection indexer (1 of 2)

تحصل وتضبط [`CellWatch`](../../cellwatch/) حسب الفهرس.

```csharp
public CellWatch this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // عرض استخدام خاصية Item
            CellWatch cellWatch = cellWatches[watchIndex];
            
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A1";
            
            Console.WriteLine("\nModified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            workbook.Save("CellWatchCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CellWatchCollection indexer (2 of 2)

تحصل وتضبط [`CellWatch`](../../cellwatch/) حسب اسم الخلية.

```csharp
public CellWatch this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف مراقبة خلية إلى المجموعة
                int watchIndex = worksheet.CellWatches.Add("A1");

                // الوصول إلى CellWatchCollection
                CellWatchCollection cellWatches = worksheet.CellWatches;

                // أظهر كيفية الوصول إلى خاصية Item باستخدام الفهرس
                CellWatch cellWatch = cellWatches[watchIndex];

                // عرض خصائص عنصر CellWatch
                Console.WriteLine("Cell Watch Details:");
                Console.WriteLine($"Row: {cellWatch.Row}");
                Console.WriteLine($"Column: {cellWatch.Column}");
                Console.WriteLine($"Cell Name: {cellWatch.CellName}");

                // احفظ المصنف
                workbook.Save("CellWatchItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellWatch](../../cellwatch/)
* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


