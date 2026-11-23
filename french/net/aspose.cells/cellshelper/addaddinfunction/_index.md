---
title: "CellsHelper.AddAddInFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Ajouter une fonction add-in"
type: docs
url: /fr/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Ajouter une fonction add-in.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fonction | String | Le nom de la fonction. |
| minCountOfParameters | Int32 | Nombre minimum de paramètres requis par cette fonction |
| maxCountOfParameters | Int32 | Nombre maximum de paramètres autorisés par cette fonction. |
| paramersType | ParameterType[] | Le type de paramètres attendu de la fonction |
| functionValueType | ParameterType | Le type de valeur de la fonction. |

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les méthodes WorksheetCollection.RegisterAddInFunction(). Cette méthode sera supprimée 12 mois plus tard à compter de janvier 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Définir les paramètres pour AddAddInFunction
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // Appeler la méthode AddAddInFunction
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Utiliser la fonction personnalisée dans une cellule
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Calculer les formules
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


