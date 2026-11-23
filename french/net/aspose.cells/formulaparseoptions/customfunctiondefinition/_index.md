---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaParseOptions. Définition pour l'analyse des fonctions personnalisées"
type: docs
url: /fr/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Définition pour l'analyse des fonctions personnalisées.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Remarques

Pour certaines exigences particulières, comme lors du calcul d'une fonction personnalisée dans le moteur personnalisé de l'utilisateur, certains de ses paramètres doivent être calculés en mode tableau ; l'utilisation de cette propriété permet de marquer ces paramètres comme mode tableau lors de l'analyse de la formule. Sinon, l'utilisateur devra mettre à jour ces fonctions personnalisées ultérieurement via [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) pour obtenir le même résultat.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une définition de fonction personnalisée
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Configurer les options d'analyse de formule avec une fonction personnalisée
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Utiliser une fonction personnalisée dans la formule
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Calculer le classeur pour démontrer le traitement de la fonction personnalisée
            workbook.CalculateFormula();

            // Enregistrer le résultat
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


