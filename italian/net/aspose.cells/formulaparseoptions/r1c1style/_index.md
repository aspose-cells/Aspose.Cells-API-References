---
title: "FormulaParseOptions.R1C1Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaParseOptions. Indica se la formula utilizza lo stile di riferimento R1C1. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

Indica se la formula utilizza lo stile di riferimento R1C1. Il valore predefinito è false.

```csharp
public bool R1C1Style { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyR1C1StyleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Imposta i valori per le celle di riferimento
            cells["D7"].PutValue(10);
            cells["D8"].PutValue(20);
            cells["D9"].PutValue(30);
            cells["C7"].PutValue(1);
            cells["C8"].PutValue(2);
            cells["C9"].PutValue(3);

            // Imposta la formula di matrice usando lo stile R1C1
            cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
                new FormulaParseOptions() { R1C1Style = true });

            // Genera le formule R1C1
            for (int i = 7; i < 10; i++)
            {
                Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
            }
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


