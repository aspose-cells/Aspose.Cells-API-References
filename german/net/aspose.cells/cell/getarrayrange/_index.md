---
title: "Cell.GetArrayRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell‑Methode. Gibt den Array‑Bereich zurück, wenn die Zellformel eine Array‑Formel ist"
type: docs
url: /de/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Ermittelt den Array‑Bereich, wenn die Zellformel eine Array‑Formel ist.

```csharp
public CellArea GetArrayRange()
```

### Rückgabewert

Der Array‑Bereich.

### Hinweise

Gilt nur, wenn die Zellformel eine Array‑Formel ist

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Eine dynamische Array-Formel in Zelle A1 festlegen
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Formeln berechnen
            wb.CalculateFormula();
            
            // Hole den Array‑Bereich der dynamischen Formel
            CellArea arrayRange = cell.GetArrayRange();
            
            // Gib die Informationen zum Array‑Bereich aus
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Gib die Werte im Array‑Bereich aus
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

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


