---
title: "Cell.FloatValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على القيمة العشرية الموجودة في الخلية"
type: docs
url: /ar/net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

يحصل على القيمة العائمة الموجودة في الخلية.

```csharp
public float FloatValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFloatValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // اضبط القيمة الرقمية مباشرة
            worksheet.Cells["A1"].PutValue(3.14f);
            Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
            
            // اضبط صيغة تُعيد قيمة عشرية
            worksheet.Cells["A2"].Formula = "=3.5*2";
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
            
            // عرض FloatValue باستخدام صيغة مشتركة
            worksheet.Cells["B1"].Formula = "=5-2";
            workbook.CalculateFormula();
            worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
            workbook.CalculateFormula();
            Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


