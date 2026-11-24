---
title: "CalculationOptions.Recursive"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Gibt an, ob abhängige Zellen rekursiv berechnet werden, wenn eine Zelle berechnet wird und sie von anderen Zellen abhängt. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Gibt an, ob abhängige Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. Der Standardwert ist true.

```csharp
public bool Recursive { get; set; }
```

### Beispiele

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
            
            // Zirkuläre Referenz erstellen
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Erste Berechnung mit Recursive=true (Standard)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Zweite Berechnung mit Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


