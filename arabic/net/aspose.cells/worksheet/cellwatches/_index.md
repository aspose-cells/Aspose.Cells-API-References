---
title: "Worksheet.CellWatches"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. يحصل على مجموعة الخلايا في هذه الورقة التي يتم مراقبتها في نافذة المراقبة"
type: docs
url: /ar/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

يحصل على مجموعة الخلايا في هذه الورقة التي يتم مراقبتها في 'نافذة المراقبة'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى الخلية B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // إضافة مراقبة خلية لـ B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // عرض معلومات المراقبة
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // احفظ المصنف
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


