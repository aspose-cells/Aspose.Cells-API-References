---
title: "ListColumn.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListColumn. تحصل وتضبط اسم العمود"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

يحصل على اسم العمود ويضبطه.

```csharp
public string Name { get; set; }
```

### ملاحظات

إذا تم ضبط اسم العمود، ستتغير قيمة الخلية المقابلة أيضًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // إنشاء كائن جدول/قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // الوصول وتعديل خاصية Name للعمود الأول في القائمة
            listObject.ListColumns[0].Name = "NewID";
            
            // تحقق من أن الاسم تم ضبطه
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // احفظ المصنف
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


