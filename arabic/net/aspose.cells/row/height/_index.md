---
title: "Row.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل وتعيّن ارتفاع الصف بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells/row/height/
---
## Row.Height property

يسترجع ويعيّن ارتفاع الصف بوحدة النقاط.

```csharp
public double Height { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين ارتفاع الصف للصف الأول
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // إضافة بعض البيانات إلى الصف
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // تحقق وعرض ارتفاع الصف
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // احفظ المصنف
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


