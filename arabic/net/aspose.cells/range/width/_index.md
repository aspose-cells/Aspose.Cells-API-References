---
title: "Range.Width"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تحصل على عرض النطاق بالنقاط"
type: docs
url: /ar/net/aspose.cells/range/width/
---
## Range.Width property

يحصل على عرض النطاق بالنقاط.

```csharp
public double Width { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد عرض الأعمدة لتوضيح خاصية Width
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // عرض عرض النطاق (مجموع عرض الأعمدة في النطاق)
            Console.WriteLine("Range Width: " + range.Width);
            
            // عرض الخصائص الفردية للتحقق
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


