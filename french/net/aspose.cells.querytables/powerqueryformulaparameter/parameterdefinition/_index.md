---
title: "PowerQueryFormulaParameter.ParameterDefinition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaParameter. Obtient la définition du paramètre"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

Obtient la définition du paramètre.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PowerQueryFormulaParameter.FormulaDefinition. Cette propriété sera supprimée 12 mois plus tard, à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyParameterDefinitionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accédez à la propriété DataMashup du classeur
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // Accédez à la collection PowerQueryFormulaParameters
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Parcourez les paramètres pour démontrer la propriété ParameterDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Affichez la valeur de la propriété ParameterDefinition (propriété en lecture seule)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Parameter Definition: {parameter.ParameterDefinition}");
                        Console.WriteLine($"Formula Definition: {parameter.FormulaDefinition}");
                        Console.WriteLine($"Parameter Value: {parameter.Value}");
                        Console.WriteLine("----------------------------------------");
                    }

                    if (parameters.Count == 0)
                    {
                        Console.WriteLine("No PowerQueryFormulaParameter instances found in the workbook.");
                    }
                }
                else
                {
                    Console.WriteLine("No DataMashup available in the workbook.");
                }

                // Enregistrez le classeur
                workbook.Save("ParameterDefinitionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


