---
title: "Cell.BoolValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على القيمة المنطقية الموجودة في الخلية"
type: docs
url: /ar/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

يحصل على القيمة المنطقية الموجودة في الخلية.

```csharp
public bool BoolValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // تعيين صيغة تُقيم إلى قيمة منطقية
            cell.Formula = "=2.01>2";
            
            // احسب الصيغة للحصول على النتيجة
            workbook.CalculateFormula();
            
            // عرض خاصية BoolValue
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


