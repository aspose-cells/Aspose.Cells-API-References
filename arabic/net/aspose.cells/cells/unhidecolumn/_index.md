---
title: "Cells.UnhideColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُظهر عمودًا مخفيًا"
type: docs
url: /ar/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

يكشف عن عمود

```csharp
public void UnhideColumn(int column, double width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| العرض | Double | عرض العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // إخفاء العمود 2
            cells.HideColumn(2);
            
            // إظهار العمود 2 مع تعديل العرض (-1 يعني استخدام العرض القياسي)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


