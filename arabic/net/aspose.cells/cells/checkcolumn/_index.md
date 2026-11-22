---
title: "Cells.CheckColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على عنصر Column أو null عند فهرس العمود المحدد"
type: docs
url: /ar/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

تحصل على عنصر [`Column`](../../column/) أو null عند فهرس العمود المحدد.

```csharp
public Column CheckColumn(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |

### قيمة الإرجاع

كائن Column.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // تعيين قيمة في العمود 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // تحقق من العمود 4 (العمود E)
            Column column = cells.CheckColumn(4);
            
            // إخراج خصائص العمود
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### انظر أيضًا

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


