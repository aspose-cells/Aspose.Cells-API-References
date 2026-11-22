---
title: "ListObject.DisplayName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل على اسم العرض للجدول ويضبطه"
type: docs
url: /ar/net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

يحصل ويضبط اسم العرض للجدول.

```csharp
public string DisplayName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // ضبط اسم العرض وعرض استخدامه
            listObject.DisplayName = "ProductTable";
            Console.WriteLine("List Object Display Name: " + listObject.DisplayName);

            // احفظ المصنف
            workbook.Save("ListObjectDisplayNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


