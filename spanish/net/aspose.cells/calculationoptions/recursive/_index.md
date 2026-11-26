---
title: "CalculationOptions.Recursive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. Indica si se calculan las celdas dependientes de forma recursiva al calcular una celda que depende de otras celdas. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Indica si se deben calcular recursivamente las celdas dependientes al calcular una celda que depende de otras celdas. El valor predeterminado es true.

```csharp
public bool Recursive { get; set; }
```

### Ejemplos

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
            
            // Crear referencia circular
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Primer cálculo con Recursive=true (predeterminado)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Segundo cálculo con Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


