---
title: "CellWatch.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellWatch. تحصل وتضبط صف الخلية"
type: docs
url: /ar/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

يحصل على صف الخلية ويضبطه.

```csharp
public int Row { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى الخلية B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // أضف CellWatch للخلية B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // عرض خاصية Row
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // تحقق من مرجع الخلية
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


