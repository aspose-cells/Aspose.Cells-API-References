---
title: "Cells.InsertRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُدرج صفًا جديدًا في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

يدرج صفًا جديدًا في ورقة العمل.

```csharp
public void InsertRow(int rowIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // احصل على مجموعة الخلايا
            Cells cells = sheet.Cells;
            
            // أدرج بيانات نموذجية في الصف 6
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // أدرج بيانات نموذجية في الصف 7
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // أدرج صفًا جديدًا عند الفهرس 7 (يدفع الصف 7 الحالي إلى الأسفل)
            cells.InsertRow(7);
            
            // أضف بيانات إلى الصف الذي تم إدراجه حديثًا
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // احفظ المصنف
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


