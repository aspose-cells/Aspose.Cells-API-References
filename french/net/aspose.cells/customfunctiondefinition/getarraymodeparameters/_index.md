---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomFunctionDefinition. Obtient les indices des paramètres des fonctions personnalisées donnés qui doivent être calculés en mode tableau"
type: docs
url: /fr/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Obtient les indices des paramètres de la fonction personnalisée donnée qui doivent être calculés en mode tableau.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| functionName | String | Nom de la fonction personnalisée. |

### Valeur de retour

Indices des paramètres qui doivent être calculés en mode tableau pour la fonction personnalisée donnée. La valeur par défaut est null, aucun paramètre n'a besoin d'être calculé en mode tableau pour la fonction personnalisée.

### Remarques

Pour une expression qui doit être calculée, en prenant A:A+B:B comme exemple : généralement en mode valeur, elle sera calculée en une seule valeur selon la base de la cellule actuelle. Mais en mode tableau, toutes les valeurs de A1+B1, A2+B2, A3+B3, … seront calculées et utilisées pour le calcul.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de CustomFunctionDefinition
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // Appeler GetArrayModeParameters avec un paramètre de nom de fonction
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Afficher le résultat
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


