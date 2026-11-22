---
title: "ListObject.AlternativeText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل وتعيّن النص البديل"
type: docs
url: /ar/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

يحصل ويضبط النص البديل.

```csharp
public string AlternativeText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء كائن/جدول قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // تعيين النص البديل والوصف
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // أعد التحميل وتحقق
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


