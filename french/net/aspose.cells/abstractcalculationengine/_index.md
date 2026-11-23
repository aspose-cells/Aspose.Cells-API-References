---
title: "Classe AbstractCalculationEngine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.AbstractCalculationEngine class. Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells"
type: docs
url: /fr/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Indique si ce moteur a besoin que le paramètre soit calculé en mode tableau. La valeur par défaut est false. Si [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) est requis lors du calcul de fonctions personnalisées et que l'utilisateur n'a pas mis à jour la définition pour celles‑ci (via [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), cette propriété doit être définie sur true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Indique si ce moteur a besoin du texte littéral du paramètre lors d'un calcul. La valeur par défaut est false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Indique si les fonctions intégrées prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation. La valeur par défaut est false. |

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Calcule une fonction avec les données fournies. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Indique s'il faut forcer la fonction donnée à être recalculée à chaque fois lors du calcul des formules partagées. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Ignore le calcul de toute la formule qui fait référence à la fonction actuellement évaluée. |

### Remarques

L'utilisateur ne doit pas modifier directement aucune partie du classeur dans cette implémentation (excepté le résultat calculé de la fonction personnalisée, qui peut être défini via la propriété CalculationData.CalculatedValue). Sinon, un résultat inattendu ou une Exception peut survenir. Si l'utilisateur doit modifier d'autres données que le résultat calculé dans l'implémentation pour certaines fonctions personnalisées, par exemple modifier la formule d'une cellule, le style, etc., il doit rassembler ces données dans cette implémentation et les modifier en dehors du périmètre du calcul de formule.

### Exemples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Exemple : implémentation personnalisée pour une fonction nommée "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // En supposant que MYFUNC prend deux paramètres et renvoie leur somme
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Forcer le recalcul pour la fonction personnalisée "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Insérez quelques valeurs dans les cellules
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Ajoutez une formule qui utilise la fonction personnalisée
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Définissez les options de calcul avec le moteur personnalisé
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Calculez les formules avec le moteur personnalisé
            workbook.CalculateFormula(options);

            // Affichez le résultat de la fonction personnalisée
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Enregistrez le classeur
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


