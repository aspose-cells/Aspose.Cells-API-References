---
title: "Worksheet.HasAutofilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كانت هذه ورقة العمل تحتوي على مرشح تلقائي"
type: docs
url: /ar/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

يشير إلى ما إذا كانت ورقة العمل هذه تحتوي على مرشح تلقائي.

```csharp
public bool HasAutofilter { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // تعيين مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:B3";
            
            // تحقق مما إذا كانت ورقة العمل تحتوي على مرشح تلقائي
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


