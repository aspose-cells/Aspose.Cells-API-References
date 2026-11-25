---
title: "CalculationOptions.Recursive"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Indica se calcolare le celle dipendenti in modo ricorsivo quando si calcola una cella e questa dipende da altre celle. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle. Il valore predefinito è true.

```csharp
public bool Recursive { get; set; }
```

### Esempi

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
            
            // Crea un riferimento circolare
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Primo calcolo con Recursive=true (predefinito)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Secondo calcolo con Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


