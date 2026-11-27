---
title: "Cell.GetDependentsInCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar alla celler vars beräknade resultat beror på denna cell"
type: docs
url: /sv/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Hämtar alla celler vars beräknade resultat beror på denna cell.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rekursiv | Boolean | Om den returnerar de beroende som inte refererar direkt till denna cell utan refererar till andra löv av denna cell |

### Returvärde

Enumerator för att enumerera alla beroende (Cell-objekt)

### Anmärkningar

För att använda denna metod, se till att arbetsboken har satts till true för [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) och har beräknats fullt med denna inställning. Om det inte finns någon formelreferens till denna cell, returneras null.

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


