---
title: "Row.LastDataCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل على آخر خلية غير فارغة في الصف"
type: docs
url: /ar/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

يسترجع آخر خلية غير فارغة في الصف.

```csharp
public Cell LastDataCell { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // إدخال البيانات في الخلايا
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // الحصول على آخر خلية بيانات في الصف الأول
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


