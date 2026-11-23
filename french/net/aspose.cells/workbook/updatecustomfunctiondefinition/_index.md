---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Met à jour la définition des fonctions personnalisées"
type: docs
url: /fr/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Met à jour la définition des fonctions personnalisées.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Définition spéciale des fonctions personnalisées pour le besoin particulier de l'utilisateur. |

### Remarques

Cette méthode peut être utilisée pour certains scénarios spéciaux. Par exemple, si l'utilisateur a besoin que certains paramètres de fonctions personnalisées soient calculés en mode tableau, il peut fournir sa propre définition avec l'implémentation de [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) pour ces fonctions. Après la mise à jour des données des formules, ces paramètres spécifiés seront calculés automatiquement en mode tableau lors du calcul des fonctions personnalisées correspondantes.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Créer un moteur de calcul personnalisé
            var customEngine = new MyCustomCalculationEngine();
            
            // Définir les options de calcul avec un moteur personnalisé
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Mettre à jour la définition de la fonction personnalisée
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Définir la formule en utilisant la fonction personnalisée
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Calculer les formules
            wb.CalculateFormula(options);

            // Afficher le résultat
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Retourner les indices des paramètres qui doivent être traités en mode tableau
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### Voir aussi

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


