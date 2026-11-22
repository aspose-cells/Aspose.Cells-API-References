---
title: "ListObject.Comment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل وتعيّن تعليق الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

يحصل ويضبط تعليق الجدول.

```csharp
public string Comment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لكائن القائمة
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(100);

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];

            // تعيين وعرض خاصية Comment
            listObj.Comment = "This is a sample comment for the list object";
            Console.WriteLine("List Object Comment: " + listObj.Comment);

            // تغيير حجم كائن القائمة لتضمين المزيد من البيانات
            listObj.Resize(0, 0, 2, 1, true);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(200);

            // احفظ المصنف
            workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


