---
title: "Cell.GetDependentsInCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient toutes les cellules dont le résultat calculé dépend de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Obtient toutes les cellules dont le résultat calculé dépend de cette cellule.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| recursive | Boolean | Renvoie les dépendants qui ne font pas référence directement à cette cellule mais font référence à d'autres feuilles de cette cellule |

### Valeur de retour

Énumérateur pour énumérer tous les dépendants (objets Cell)

### Remarques

Pour utiliser cette méthode, veuillez vous assurer que le classeur a été configuré avec la valeur true pour [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) et qu'il a été entièrement calculé avec ce paramètre. S'il n'y a aucune référence de formule à cette cellule, null sera retourné.

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


