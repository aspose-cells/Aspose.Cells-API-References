---
title: "ListObject.StartRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل على الصف الابتدائي للنطاق"
type: docs
url: /ar/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

يحصل على الصف الابتدائي للنطاق.

```csharp
public int StartRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة بدءًا من الصف 2
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // إنشاء كائن قائمة بدءًا من الصف 2
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // عرض خاصية StartRow
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // لت \"تعديل\" الصف الابتدائي، نحتاج إلى إعادة إنشاء ListObject
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


