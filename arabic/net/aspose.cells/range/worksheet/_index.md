---
title: "Range.Worksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تحصل على كائن Worksheet الذي يحتوي على هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

يحصل على كائن `Worksheet` الذي يحتوي على هذا النطاق.

```csharp
public Worksheet Worksheet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق مسمى
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // تعريف نطاق مسمى
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // احصل على النطاق بالاسم (حدد Range بالكامل لتجنب الغموض)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // عرض كيفية استخدام خاصية Worksheet
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // استخدم خاصية Worksheet لتعديل الخلايا
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // احفظ المصنف
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


