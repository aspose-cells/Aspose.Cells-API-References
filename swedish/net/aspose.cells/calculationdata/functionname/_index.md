---
title: "CalculationData.FunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData-egenskap. Hämtar funktionsnamnet som ska beräknas"
type: docs
url: /sv/net/aspose.cells/calculationdata/functionname/
---
## CalculationData.FunctionName property

Hämtar funktionsnamnet som ska beräknas.

```csharp
public string FunctionName { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyFunctionNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";
            
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new MyCustomEngine();
            workbook.CalculateFormula(options);
            
            Console.WriteLine("Custom function result: " + sheet.Cells["A3"].Value);
        }
    }

    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                double param1 = Convert.ToDouble(((ReferredArea)data.GetParamValue(0)).GetValue(0, 0));
                double param2 = Convert.ToDouble(((ReferredArea)data.GetParamValue(1)).GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }
    }
}
```

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


