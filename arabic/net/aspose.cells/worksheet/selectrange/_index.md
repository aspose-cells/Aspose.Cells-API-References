---
title: "Worksheet.SelectRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تختار نطاقًا"
type: docs
url: /ar/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

يحدد نطاقًا.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | صف البداية. |
| startColumn | Int32 | عمود البداية |
| totalRows | Int32 | عدد الصفوف. |
| totalColumns | Int32 | عدد الأعمدة |
| removeOthers | منطقي | True يعني إزالة النطاق المحدد الآخر واختيار هذا النطاق فقط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد النطاق من الصف 1، العمود 1 إلى الصف 5، العمود 5 (B2:F6) واجعله نشطًا
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


