---
title: "Énumération CalculationPrecisionStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.CalculationPrecisionStrategy. Énumère les stratégies de gestion de la précision des calculs. En raison du problème de précision de l'arithmétique à virgule flottante IEEE 754, certaines formules apparemment simples peuvent ne pas être calculées comme le résultat attendu. Par exemple, la formule 0.450.430.02 lorsqu'on calcule les opérandes directement avec l'opérateur, le résultat n'est pas zéro. Pour ce type de problème de précision, certaines stratégies spéciales peuvent fournir le résultat attendu."
type: docs
url: /fr/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

Énumère les stratégies de gestion de la précision des calculs. En raison du problème de précision de l'arithmétique à virgule flottante IEEE 754, certaines formules « apparemment simples » peuvent ne pas être calculées avec le résultat attendu. Par exemple, la formule "=-0.45+0.43+0.02", lorsqu'on calcule les opérandes directement avec l'opérateur '+', le résultat n'est pas zéro. Pour ce type de problème de précision, certaines stratégies spéciales peuvent fournir le résultat attendu.

```csharp
public enum CalculationPrecisionStrategy
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucune stratégie appliquée au calcul. Lors du calcul, utilisez simplement la valeur double originale comme opérande et renvoyez le résultat directement. C’est la solution la plus efficace en termes de performances et applicable dans la plupart des cas. |
| Round | `1` | Arrondit le résultat du calcul selon les chiffres significatifs. |
| Decimal | `2` | Utilise le type décimal comme opérandes lorsque cela est possible. C’est le moins efficace en termes de performances. |

### Exemples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Définissez les options de calcul
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Calculer les formules dans la feuille de calcul
            workbook.CalculateFormula(calcOptions);

            // Obtenir le résultat de la formule
            double result = worksheet.Cells["A2"].DoubleValue;

            // Afficher le résultat
            Console.WriteLine("Calculated Result: " + result);

            // Enregistrez le classeur
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


