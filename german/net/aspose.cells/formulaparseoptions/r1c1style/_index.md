---
title: "FormulaParseOptions.R1C1Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaParseOptions-Eigenschaft. Gibt an, ob die Formel im R1C1-Referenzstil vorliegt. Standard ist false"
type: docs
url: /de/net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

Ob die Formel im R1C1-Bezugsstil vorliegt. Standard ist false.

```csharp
public bool R1C1Style { get; set; }
```

### Beispiele

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

            // Werte für referenzierte Zellen festlegen
            cells["D7"].PutValue(10);
            cells["D8"].PutValue(20);
            cells["D9"].PutValue(30);
            cells["C7"].PutValue(1);
            cells["C8"].PutValue(2);
            cells["C9"].PutValue(3);

            // Array-Formel im R1C1-Stil festlegen
            cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
                new FormulaParseOptions() { R1C1Style = true });

            // Geben Sie die R1C1-Formeln aus
            for (int i = 7; i < 10; i++)
            {
                Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
            }
        }
    }
}
```

### Siehe auch

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


