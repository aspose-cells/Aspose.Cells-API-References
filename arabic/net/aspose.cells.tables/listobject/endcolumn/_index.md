---
title: "ListObject.EndColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل على العمود النهائي للنطاق"
type: docs
url: /ar/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

يحصل على العمود النهائي للنطاق.

```csharp
public int EndColumn { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // إنشاء كائن/جدول قائمة
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // عرض العمود النهائي الأصلي
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // تغيير حجم الجدول لتضمين عمود إضافي
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // عرض العمود النهائي الجديد
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // احفظ المصنف
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


