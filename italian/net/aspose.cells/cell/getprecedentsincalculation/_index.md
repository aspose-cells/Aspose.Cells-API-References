---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene tutti i riferimenti ai precedenti delle celle nel workbook corrente usati dalla formula di questa cella durante il calcolo"
type: docs
url: /it/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Ottiene tutti i precedenti (riferimento a celle nella cartella di lavoro corrente) utilizzati dalla formula di questa cella durante il calcolo.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Valore di ritorno

Enumeratore per enumerare tutti i riferimenti (ReferredArea)

### Osservazioni

Questo metodo può funzionare solo nella situazione in cui [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) è impostato su true per il workbook e il workbook è stato completamente calcolato. Se questa cella non è una formula o non fa riferimento a nessun'altra cella, verrà restituito null.

### Esempi

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

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


