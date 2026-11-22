---
title: "Cell.DateTimeValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. يحصل على قيمة DateTime الموجودة في الخلية"
type: docs
url: /ar/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

يحصل على قيمة DateTime الموجودة في الخلية.

```csharp
public DateTime DateTimeValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // حدد قيمة DateTime في الخلية A1
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // نسق الخلية لعرض التاريخ
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // استرجع وتحقق من قيمة DateTimeValue
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // حدد قيمة DateTime أخرى في الخلية B1
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // اعرض قيمة DateTimeValue من B1
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


