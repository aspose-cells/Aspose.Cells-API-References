---
title: "FindOptions.SearchBackward"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FindOptions. ما إذا كان البحث يتم للخلف عن الخلايا"
type: docs
url: /ar/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

ما إذا كان البحث عكسيًا للخلايا.

```csharp
public bool SearchBackward { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إعداد بيانات عينة
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // البحث إلى الأمام (السلوك الافتراضي)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // بحث إلى الخلف
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### انظر أيضًا

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


