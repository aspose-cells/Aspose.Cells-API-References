---
title: "Cell.GetArrayRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell metod. Hämtar matrisområdet om cellens formel är en matrisformel"
type: docs
url: /sv/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Hämtar array-intervallet om cellens formel är en arrayformel.

```csharp
public CellArea GetArrayRange()
```

### Returvärde

Matrisområdet.

### Anmärkningar

Gäller endast när cellens formel är en matrisformel

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Ställ in en dynamisk arrayformel i cell A1
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Beräkna formler
            wb.CalculateFormula();
            
            // Hämta arrayområdet för den dynamiska formeln
            CellArea arrayRange = cell.GetArrayRange();
            
            // Skriv ut information om arrayområdet
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Skriv ut värdena i arrayområdet
            Console.WriteLine("\nValues in the array range:");
            for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
            {
                for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
                {
                    Console.Write(cells[r, c].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


