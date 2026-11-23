---
title: "Cells.GetDependents"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Récupère toutes les cellules qui font référence à la cellule spécifique"
type: docs
url: /fr/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Obtient toutes les cellules qui font référence à la cellule spécifique.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isAll | Boolean | Indique s'il faut vérifier les autres feuilles de calcul |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Configurer des formules et des valeurs d'exemple
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Calculer les formules
            workbook.CalculateFormula();

            // Obtenir les dépendants directs de la cellule A1 (ligne 0, colonne 0)
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // Obtenir tous les dépendants (y compris indirects) de la cellule A1 (ligne 0, colonne 0)
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


