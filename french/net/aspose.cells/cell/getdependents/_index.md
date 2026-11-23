---
title: "Cell.GetDependents"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Récupère toutes les cellules dont la formule fait référence directement à cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Obtenir toutes les cellules dont la formule fait référence directement à cette cellule.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isAll | Boolean | Indique si les formules sont vérifiées dans d'autres feuilles de calcul |

### Remarques

Si une référence contenant cette cellule apparaît dans la formule d’une cellule, cette cellule sera considérée comme dépendante de cette cellule, que la référence ou cette cellule soit utilisée ou non lors du calcul. Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul, cette formule sera quand même considérée comme dépendante de A2. Pour obtenir les formules dont les résultats calculés dépendent de cette cellule, veuillez utiliser [`GetDependentsInCalculation`](../getdependentsincalculation/). Lors du suivi des dépendants pour une cellule, toutes les formules du classeur ou de la feuille de calcul seront analysées et vérifiées. C’est donc un processus gourmand en temps. Si l’utilisateur doit tracer les dépendants pour de nombreuses cellules, l’utilisation de cette méthode entraînera de mauvaises performances. Pour des raisons de performance, l’utilisateur devrait plutôt utiliser [`GetDependentsInCalculation`](../getdependentsincalculation/). Ou bien, l’utilisateur peut d’abord rassembler la carte des précédents de toutes les cellules avec [`GetPrecedents`](../getprecedents/), puis construire la carte des dépendants à partir de la carte des précédents.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir des formules qui font référence à B1
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Calculer les formules
            workbook.CalculateFormula();

            // Obtenir toutes les cellules qui dépendent de B1 (récursif)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


