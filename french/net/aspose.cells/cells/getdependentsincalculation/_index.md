---
title: "Cells.GetDependentsInCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient toutes les cellules dont le résultat calculé dépend d'une cellule spécifique"
type: docs
url: /fr/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Obtient toutes les cellules dont le résultat calculé dépend de la cellule spécifique.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de la cellule spécifique |
| column | Int32 | Indice de colonne de la cellule spécifique. |
| recursive | Boolean | Indique si la méthode renvoie les dépendants qui ne font pas référence directement à la cellule spécifique mais à d'autres feuilles de cette cellule. |

### Valeur de retour

Énumérateur pour énumérer tous les dépendants (objets Cell)

### Remarques

Pour utiliser cette méthode, veuillez vous assurer que le classeur a été configuré avec la valeur true pour [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) et a été entièrement calculé avec ce paramètre. S'il n'y a aucune référence de formule à cette cellule, null sera renvoyé. Pour plus de détails et un exemple, veuillez consulter [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/)

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et calculez les formules
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Configurez les dépendances de formules :
            // C1 = 10 (valeur source)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Calculez les formules pour établir les dépendances
            workbook.CalculateFormula();

            try
            {
                // Obtenez les dépendants de la cellule C1 (ligne 0, colonne 2) avec vérification récursive
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


