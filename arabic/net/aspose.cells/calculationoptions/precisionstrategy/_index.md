---
title: "CalculationOptions.PrecisionStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. يحدد الاستراتيجية لمعالجة دقة الحساب"
type: docs
url: /ar/net/aspose.cells/calculationoptions/precisionstrategy/
---
## CalculationOptions.PrecisionStrategy property

يحدد الاستراتيجية لمعالجة دقة الحساب.

```csharp
public CalculationPrecisionStrategy PrecisionStrategy { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyPrecisionStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(1.23456789);
            worksheet.Cells["A2"].PutValue(2.34567891);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            CalculationOptions calcOptions = new CalculationOptions
            {
                PrecisionStrategy = CalculationPrecisionStrategy.Round
            };

            workbook.CalculateFormula(calcOptions);

            Console.WriteLine("A3 calculated value with Round strategy: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### انظر أيضًا

* enum [CalculationPrecisionStrategy](../../calculationprecisionstrategy/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


