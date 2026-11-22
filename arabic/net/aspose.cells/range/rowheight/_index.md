---
title: "Range.RowHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تُعيّن أو تُعيد ارتفاع الصفوف في هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق

```csharp
public double RowHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ضع بعض البيانات في الصف الأول
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // احصل على ارتفاع الصف الأولي
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // اضبط الصف تلقائيًا
            worksheet.AutoFitRow(0);

            // احصل على ارتفاع الصف الجديد بعد الضبط التلقائي
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // قم بتعيين ارتفاع صف جديد يدويًا
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


