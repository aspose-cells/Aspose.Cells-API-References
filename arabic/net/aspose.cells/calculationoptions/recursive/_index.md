---
title: "CalculationOptions.Recursive"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. تشير إلى ما إذا كان يتم حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

يشير إلى ما إذا كان يتم حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. القيمة الافتراضية هي true.

```csharp
public bool Recursive { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyRecursiveDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // إنشاء إشارة دائرية
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // الحساب الأول مع Recursive=true (الافتراضي)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // الحساب الثاني مع Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


