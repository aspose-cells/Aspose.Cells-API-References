---
title: "Range.RefersTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على النطاقات التي يشير إليها"
type: docs
url: /ar/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

يحصل على ما يشير إليه النطاق.

```csharp
public string RefersTo { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // إنشاء نطاق مسمى
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // تعيين خاصية RefersTo للنطاق المسمى
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // الحصول على النطاقات المشار إليها بالاسم
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // عرض خاصية RefersTo للنطاق الأول
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // إنشاء صيغة تستخدم النطاق المسمى
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // احسب الصيغة
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


