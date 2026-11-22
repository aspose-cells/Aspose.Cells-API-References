---
title: "Cells.IsRowHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا"
type: docs
url: /ar/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا.

```csharp
public bool IsRowHidden(int rowIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف |

### قيمة الإرجاع

صحيح إذا كان الصف مخفيًا

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // بيانات عينة
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // تطبيق الفلتر
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // تحقق من رؤية الصف
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


