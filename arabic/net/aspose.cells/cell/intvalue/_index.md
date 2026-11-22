---
title: "Cell.IntValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على القيمة الصحيحة الموجودة في الخلية"
type: docs
url: /ar/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

يحصل على القيمة الصحيحة الموجودة في الخلية.

```csharp
public int IntValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // تعيين قيمة رقمية والحصول على IntValue
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // تعيين صيغة تُقيم إلى رقم والحصول على IntValue
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // تعيين قيمة منطقية والحصول على IntValue
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // تعيين قيمة نصية والحصول على IntValue (سيكون 0 إذا لم يكن قابلاً للتحويل)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


