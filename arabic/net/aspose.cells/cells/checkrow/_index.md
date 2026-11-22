---
title: "Cells.CheckRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على عنصر Row أو null عند فهرس صف الخلية المحدد"
type: docs
url: /ar/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

يحصل على عنصر [`Row`](../../row/) أو null عند فهرس صف الخلية المحدد.

```csharp
public Row CheckRow(int row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف |

### قيمة الإرجاع

يرجع كائن [`Row`](../../row/) إذا كان كائن الصف موجودًا، وإلا يرجع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // ملء بعض البيانات
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // تحقق مما إذا كان الصف موجودًا واحصل على كائن الصف
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // تحقق من صف غير موجود
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### انظر أيضًا

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


