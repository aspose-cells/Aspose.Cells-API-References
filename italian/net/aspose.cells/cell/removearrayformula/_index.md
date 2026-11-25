---
title: "Cell.RemoveArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Rimuove la formula array"
type: docs
url: /it/net/aspose.cells/cell/removearrayformula/
---
## Cell.RemoveArrayFormula method

Rimuove la formula di matrice.

```csharp
public void RemoveArrayFormula(bool leaveNormalFormula)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| leaveNormalFormula | Booleano | True indica la conversione della formula array in formula normale. |

### Esempi

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

            // Imposta la formula array in una singola cella
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

            // Imposta nuovamente la formula array e rimuovi con il parametro true
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter RemoveArrayFormula(true):");
            Console.WriteLine("IsArrayHeader: " + cell.IsArrayHeader);
            Console.WriteLine("Formula: " + cell.Formula);

            // Imposta la formula array su più celle
            cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(false):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Value = {cells[0, i].Value}");
            }

            // Imposta nuovamente la formula array e rimuovi con il parametro true
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

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


