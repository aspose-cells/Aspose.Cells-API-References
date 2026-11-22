---
title: "Row.IsBlank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تشير إلى ما إذا كان الصف يحتوي على أي بيانات"
type: docs
url: /ar/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

يشير إلى ما إذا كان الصف يحتوي على أي بيانات

```csharp
public bool IsBlank { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على الصف الأول (فارغ في البداية)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // إضافة بيانات إلى الصف الأول
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // إنشاء صف فارغ آخر
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // مقارنة حالة فراغ الصف
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


