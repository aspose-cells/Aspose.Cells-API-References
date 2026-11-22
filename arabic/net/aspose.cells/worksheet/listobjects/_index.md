---
title: "Worksheet.ListObjects"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على جميع ListObjects في هذه الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

يحصل على جميع ListObjects في ورقة العمل هذه.

```csharp
public ListObjectCollection ListObjects { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // إنشاء ListObject (جدول)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // تغيير حجم الجدول لتضمين المزيد من الصفوف
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // أضف المزيد من البيانات إلى الجدول الموسع
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // الوصول إلى الجدول عبر خاصية ListObjects
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // احفظ المصنف
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


