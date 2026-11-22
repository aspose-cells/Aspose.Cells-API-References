---
title: "Cell.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخلية. تحصل على رقم الصف صفر بناءً على الخلية"
type: docs
url: /ar/net/aspose.cells/cell/row/
---
## Cell.Row property

يحصل على رقم الصف (مبني على الصفر) للخلية.

```csharp
public int Row { get; }
```

### Property Value

رقم صف الخلية

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية وصيغة
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // ابحث عن الخلية التي تحتوي على الصيغة
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // عرض خاصية Row
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // تحقق من صحة الصف
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


