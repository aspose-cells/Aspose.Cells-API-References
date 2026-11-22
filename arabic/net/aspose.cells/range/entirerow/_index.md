---
title: "Range.EntireRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على كائن Range يمثل الصف الكامل أو الصفوف التي تحتوي على النطاق المحدد"
type: docs
url: /ar/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

يحصل على كائن Range يمثل الصف بالكامل (أو الصفوف) الذي يحتوي على النطاق المحدد.

```csharp
public Range EntireRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // املأ بعض البيانات النموذجية في الصف الأول
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // احصل على الصف الأول بالكامل باستخدام خاصية EntireRow
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // انسخ الصف الأول إلى الصف الثالث
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // احفظ المصنف
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


