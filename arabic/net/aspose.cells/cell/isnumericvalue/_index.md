---
title: "Cell.IsNumericValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت قيمة هذه الخلية رقمية أو مزدوجة وتاريخ/وقت"
type: docs
url: /ar/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

يشير إلى ما إذا كانت قيمة هذه الخلية عددية (int, double و datetime)

```csharp
public bool IsNumericValue { get; }
```

### ملاحظات

ينطبق أيضًا على خلية الصيغة للتحقق من النتيجة المحسوبة

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة أنواع مختلفة من البيانات إلى الخلايا
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // تحقق مما إذا كانت الخلايا تحتوي على قيم رقمية
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // عرض الاستخدام مع المنطق الشرطي
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


