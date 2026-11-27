---
title: "Cell.RemoveArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Ta bort matrisformel"
type: docs
url: /sv/net/aspose.cells/cell/removearrayformula/
---
## Cell.RemoveArrayFormula method

Ta bort matrisformel.

```csharp
public void RemoveArrayFormula(bool leaveNormalFormula)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| leaveNormalFormula | Boolean | True representerar konvertering av matrisformeln till normal formel. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodRemoveArrayFormulaWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ställ in matrisformel i en enskild cell
            Cell cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cells["B1"].PutValue(10);
            cells["C1"].PutValue(20);
            cells["D1"].PutValue(30);
            wb.CalculateFormula();

            Console.WriteLine("Before RemoveArrayFormula(false):");
            Console.WriteLine("IsArrayFormula: " + cell.IsArrayFormula);
            Console.WriteLine("Value: " + cell.Value);

            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter RemoveArrayFormula(false):");
            Console.WriteLine("IsFormula: " + cell.IsFormula);
            Console.WriteLine("Value: " + cell.Value);

            // Ställ in matrisformel igen och ta bort med true-parameter
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter RemoveArrayFormula(true):");
            Console.WriteLine("IsArrayHeader: " + cell.IsArrayHeader);
            Console.WriteLine("Formula: " + cell.Formula);

            // Ställ in matrisformel över flera celler
            cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(false):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Value = {cells[0, i].Value}");
            }

            // Ställ in matrisformel igen och ta bort med true-parameter
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(true):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Formula = {cells[0, i].Formula}");
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


