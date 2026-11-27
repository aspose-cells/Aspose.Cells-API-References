---
title: "Enum ConsolidationFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ConsolidationFunction enum. Representerar konsolideringsfunktion"
type: docs
url: /sv/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Representerar konsolideringsfunktion.

```csharp
public enum ConsolidationFunction
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Sum | `0` | Representerar Sum-funktionen. |
| Count | `1` | Representerar Count-funktionen. |
| Average | `2` | Representerar Average-funktionen. |
| Max | `3` | Representerar Max-funktionen. |
| Min | `4` | Representerar Min-funktionen. |
| Product | `5` | Representerar Product-funktionen. |
| CountNums | `6` | Representerar Count Nums-funktionen. |
| StdDev | `7` | Representerar StdDev-funktionen. |
| StdDevp | `8` | Representerar StdDevp-funktionen. |
| Var | `9` | Representerar Var-funktionen. |
| Varp | `10` | Representerar Varp-funktionen. |
| DistinctCount | `11` | Representerar Distinct Count-funktionen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Definiera cellområdet för delsumma
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Applicera delsumma med Sum-funktionen
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Applicera delsumma med Average-funktionen
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Applicera delsumma med Max-funktionen
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Applicera delsumma med Min-funktionen
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Spara arbetsboken
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Skriv ut resultaten
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


