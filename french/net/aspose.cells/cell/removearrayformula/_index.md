---
title: "Cell.RemoveArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Supprimer la formule matricielle"
type: docs
url: /fr/net/aspose.cells/cell/removearrayformula/
---
## Cell.RemoveArrayFormula method

Supprime la formule de tableau.

```csharp
public void RemoveArrayFormula(bool leaveNormalFormula)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | Boolean | True représente la conversion de la formule matricielle en formule normale. |

### Exemples

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

            // Définir la formule matricielle dans une seule cellule
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

            // Définir à nouveau la formule matricielle et la supprimer avec le paramètre true
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter RemoveArrayFormula(true):");
            Console.WriteLine("IsArrayHeader: " + cell.IsArrayHeader);
            Console.WriteLine("Formula: " + cell.Formula);

            // Définir la formule matricielle sur plusieurs cellules
            cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(false):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Value = {cells[0, i].Value}");
            }

            // Définir à nouveau la formule matricielle et la supprimer avec le paramètre true
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

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


