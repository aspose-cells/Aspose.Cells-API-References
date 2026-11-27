---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Hämtar alla föregångarreferenser till celler i den aktuella arbetsboken som används av den här cellens formel vid beräkning."
type: docs
url: /sv/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Hämtar alla föregångare (referens till celler i aktuell arbetsbok) som används av cellens formel vid beräkning.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Returvärde

Enumerator för att enumerera alla referenser (ReferredArea)

### Anmärkningar

Denna metod kan endast fungera när situationen är att [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) är sann för arbetsboken och arbetsboken har beräknats fullt ut. Om den här cellen inte är en formel eller den inte refererar till några andra celler, returneras null.

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


