---
title: "Range.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تحصل على عرض النطاق بالنقاط"
type: docs
url: /ar/net/aspose.cells/range/height/
---
## Range.Height property

يحصل على عرض النطاق بالنقاط.

```csharp
public double Height { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين ارتفاعات الصفوف للعرض
            worksheet.Cells.SetRowHeight(1, 15.0); // Row 2 (0-based index 1)
            worksheet.Cells.SetRowHeight(2, 20.0); // Row 3
            worksheet.Cells.SetRowHeight(3, 25.0); // Row 4

            // إنشاء نطاق يمتد عبر الصفوف 2-4 (B2:C4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // عرض خاصية Height
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Calculated Height (sum of row heights): " + 
                (worksheet.Cells.GetRowHeight(1) + 
                 worksheet.Cells.GetRowHeight(2) + 
                 worksheet.Cells.GetRowHeight(3)));
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


