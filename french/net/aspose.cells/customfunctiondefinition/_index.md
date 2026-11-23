---
title: "Classe CustomFunctionDefinition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CustomFunctionDefinition. Définition d'une fonction personnalisée pour le calcul avec le moteur personnalisé de l'utilisateur"
type: docs
url: /fr/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Définition d'une fonction personnalisée pour le calcul avec le moteur personnalisé de l'utilisateur.

```csharp
public class CustomFunctionDefinition
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Obtient les indices des paramètres de la fonction personnalisée donnée qui doivent être calculés en mode tableau. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une nouvelle instance de CustomFunctionDefinition
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Créer une nouvelle instance de FormulaParseOptions et définir le CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Ajouter une feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir une formule personnalisée
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Analyser la formule personnalisée en utilisant FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Enregistrez le classeur
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


