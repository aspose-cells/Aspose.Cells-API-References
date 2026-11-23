---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaParameter. Obtient la définition du paramètre"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Obtient la définition du paramètre.

```csharp
public override string FormulaDefinition { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyFormulaDefinitionDemo
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

                    // Itérer à travers les paramètres pour démontrer FormulaDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Afficher la valeur de la propriété FormulaDefinition (propriété en lecture seule)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
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
                workbook.Save("FormulaDefinitionDemo.xlsx");
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


