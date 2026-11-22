---
title: "ListObject.EndRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل على الصف النهائي للنطاق"
type: docs
url: /ar/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

يحصل على الصف النهائي للنطاق.

```csharp
public int EndRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // إنشاء كائن قائمة/جدول
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // عرض EndRow الأولي
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // إضافة صف جديد إلى الجدول
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // عرض EndRow المحدث
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // احفظ المصنف
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


