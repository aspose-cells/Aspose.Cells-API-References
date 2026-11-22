---
title: "ListColumn.Range"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListColumn. تحصل على نطاق هذا العمود في القائمة"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

يحصل على نطاق هذا العمود في القائمة.

```csharp
public Range Range { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لإنشاء كائن قائمة
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // إنشاء كائن قائمة
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // احصل على العمود الأول في القائمة
            ListColumn listCol = listObj.ListColumns[0];
            
            // الوصول إلى نطاق عمود القائمة
            Aspose.Cells.Range range = listCol.Range;
            
            // عرض معلومات النطاق
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // تعديل الخلايا في النطاق
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // احفظ المصنف
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


