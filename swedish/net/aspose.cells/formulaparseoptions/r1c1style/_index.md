---
title: "FormulaParseOptions.R1C1Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaParseOptions egenskap. Anger om formeln är i R1C1-referensstil. Standard är falskt"
type: docs
url: /sv/net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

Om formeln använder R1C1-referensstil. Standard är false.

```csharp
public bool R1C1Style { get; set; }
```

### Exempel

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

            // Ange värden för refererade celler
            cells["D7"].PutValue(10);
            cells["D8"].PutValue(20);
            cells["D9"].PutValue(30);
            cells["C7"].PutValue(1);
            cells["C8"].PutValue(2);
            cells["C9"].PutValue(3);

            // Ange matrisformel med R1C1-stil
            cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
                new FormulaParseOptions() { R1C1Style = true });

            // Skriv ut R1C1-formlerna
            for (int i = 7; i < 10; i++)
            {
                Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
            }
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


