---
title: "Cell.GetArrayRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient la plage de tableau si la formule de la cellule est une formule matricielle"
type: docs
url: /fr/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Obtient la plage de tableau si la formule de la cellule est une formule matricielle.

```csharp
public CellArea GetArrayRange()
```

### Valeur de retour

La plage de tableau.

### Remarques

S'applique uniquement lorsque la formule de la cellule est une formule matricielle

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Définissez une formule de tableau dynamique dans la cellule A1
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Calculer les formules
            wb.CalculateFormula();
            
            // Obtenir la plage de tableau de la formule dynamique
            CellArea arrayRange = cell.GetArrayRange();
            
            // Afficher les informations de la plage de tableau
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Imprimer les valeurs dans la plage de tableau
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

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


