---
title: "FormulaParseOptions.R1C1Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormulaParseOptions. Indica si la fórmula está en estilo de referencia R1C1. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

Indica si la fórmula usa el estilo de referencia R1C1. El valor predeterminado es false.

```csharp
public bool R1C1Style { get; set; }
```

### Ejemplos

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

            // Establecer valores para celdas referenciadas
            cells["D7"].PutValue(10);
            cells["D8"].PutValue(20);
            cells["D9"].PutValue(30);
            cells["C7"].PutValue(1);
            cells["C8"].PutValue(2);
            cells["C9"].PutValue(3);

            // Establecer fórmula de matriz usando el estilo R1C1
            cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
                new FormulaParseOptions() { R1C1Style = true });

            // Generar las fórmulas R1C1
            for (int i = 7; i < 10; i++)
            {
                Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
            }
        }
    }
}
```

### Ver también

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


