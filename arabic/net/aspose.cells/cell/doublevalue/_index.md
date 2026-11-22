---
title: "Cell.DoubleValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخلية. تحصل على القيمة المزدوجة الموجودة في الخلية"
type: docs
url: /ar/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

يحصل على القيمة المزدوجة الموجودة في الخلية.

```csharp
public double DoubleValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين أنواع قيم مختلفة في الخلايا
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // عرض خاصية DoubleValue
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // التحقق من إمكانية قراءة أنواع القيم الأخرى كقيمة مزدوجة
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


