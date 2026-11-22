---
title: "Range.FirstRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على فهرس الصف الأول للنطاق"
type: docs
url: /ar/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

يحصل على فهرس الصف الأول في النطاق.

```csharp
public int FirstRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا وادخل إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء نطاق
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // ادخل واعرض خاصية FirstRow
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // ادخل إلى الخلية الأولى في الصف الأول للنطاق
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


