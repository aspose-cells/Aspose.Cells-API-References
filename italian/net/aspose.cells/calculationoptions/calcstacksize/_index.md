---
title: "CalculationOptions.CalcStackSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. La dimensione dello stack per il calcolo ricorsivo delle celle. Il valore predefinito è 200"
type: docs
url: /it/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

La dimensione dello stack per il calcolo ricorsivo delle celle. Il valore predefinito è 200.

```csharp
public int CalcStackSize { get; set; }
```

### Osservazioni

Quando vi è un grande numero di celle da calcolare ricorsivamente nell'albero delle dipendenze, potrebbe verificarsi una StackOverflowException durante il processo di calcolo. In tal caso, l'utente dovrebbe specificare un valore più piccolo per questa proprietà. Per tali situazioni, l'utente dovrebbe determinare il valore appropriato per questa proprietà in base alle formule e ai dati effettivi. Tuttavia, un valore troppo piccolo può causare un degrado delle prestazioni del calcolo delle formule e un valore inferiore a 2 renderà impossibile calcolare una formula che dipende da un'altra. Pertanto, se il valore specificato è inferiore a 2, verrà reimpostato a 2.

### Esempi

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

            // Configura formule di esempio che richiederebbero il calcolo dello stack
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Calcola con una dimensione dello stack personalizzata
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


