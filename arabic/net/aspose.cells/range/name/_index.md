---
title: "Range.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل أو يضبط اسم النطاق"
type: docs
url: /ar/net/aspose.cells/range/name/
---
## Range.Name property

يحصل أو يضبط اسم النطاق.

```csharp
public string Name { get; set; }
```

### ملاحظات

النطاق المسمى مدعوم. على سبيل المثال،

range.Name = "Sheet1!MyRange";

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق (الأعمدة A إلى B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // ضبط خاصية الاسم للنطاق
            range.Name = "testRange";
            
            // تحقق من أن الاسم تم ضبطه
            Console.WriteLine("Range name: " + range.Name);
            
            // احفظ المصنف
            workbook.Save("RangeWithName.xlsx");
            
            // افتح الملف المحفوظ لتظهر أن الاسم يبقى
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


