---
title: "FormulaParseOptions.R1C1Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaParseOptions özelliği. Formülün R1C1 referans stilinde olup olmadığını belirler. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/formulaparseoptions/r1c1style/
---
## FormulaParseOptions.R1C1Style property

Formülün R1C1 referans stilinde olup olmadığı. Varsayılan değer false'tur.

```csharp
public bool R1C1Style { get; set; }
```

### Örnekler

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

            // Referans alınan hücreler için değerleri ayarla
            cells["D7"].PutValue(10);
            cells["D8"].PutValue(20);
            cells["D9"].PutValue(30);
            cells["C7"].PutValue(1);
            cells["C8"].PutValue(2);
            cells["C9"].PutValue(3);

            // R1C1 stilini kullanarak dizi formülü ayarla
            cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
                new FormulaParseOptions() { R1C1Style = true });

            // R1C1 formüllerini çıktı al
            for (int i = 7; i < 10; i++)
            {
                Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


