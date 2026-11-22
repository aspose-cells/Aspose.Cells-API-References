---
title: "Row.FirstCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل على كائن الخلية الأولى في الصف"
type: docs
url: /ar/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

يحصل على أول كائن خلية في الصف.

```csharp
public Cell FirstCell { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات إلى الخلايا في الصف الأول
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // احصل على الصف الأول
            Row row = worksheet.Cells.Rows[0];
            
            // عرض خاصية FirstCell
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // تعديل الخلية الأولى
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // احفظ المصنف
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


