---
title: "CalculationOptions.CalcStackSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskapen. Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200"
type: docs
url: /sv/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200.

```csharp
public int CalcStackSize { get; set; }
```

### Anmärkningar

När ett stort antal celler måste beräknas rekursivt i beroendeträdet kan en StackOverflowException uppstå under beräkningsprocessen. I så fall bör användaren ange ett mindre värde för denna egenskap. I en sådan situation bör användaren bestämma rätt värde för egenskapen baserat på de faktiska formlerna och data. Dock kan ett för litet värde leda till prestandaförsämring för formelberäkningen och ett värde mindre än 2 gör det omöjligt att beräkna en formel som beror på en annan. Så om det angivna värdet är mindre än 2 kommer det att återställas till 2.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ställ in exempelformler som skulle kräva stackberäkning
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Beräkna med anpassad stackstorlek
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### Se även

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


