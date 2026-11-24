---
title: "Cell.RemoveArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Zellenmethode. Array-Formel entfernen"
type: docs
url: /de/net/aspose.cells/cell/removearrayformula/
---
## Cell.RemoveArrayFormula method

Array-Formel entfernen.

```csharp
public void RemoveArrayFormula(bool leaveNormalFormula)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| leaveNormalFormula | Boolean | True steht für die Umwandlung der Array-Formel in eine normale Formel. |

### Beispiele

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

            // Array-Formel in einer einzelnen Zelle festlegen
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

            // Array-Formel erneut festlegen und mit dem Parameter true entfernen
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter RemoveArrayFormula(true):");
            Console.WriteLine("IsArrayHeader: " + cell.IsArrayHeader);
            Console.WriteLine("Formula: " + cell.Formula);

            // Array-Formel über mehrere Zellen festlegen
            cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(false):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Value = {cells[0, i].Value}");
            }

            // Array-Formel erneut festlegen und mit dem Parameter true entfernen
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

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


