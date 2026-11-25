---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaParameter. Ottiene la definizione del parametro"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Ottiene la definizione del parametro.

```csharp
public override string FormulaDefinition { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla proprietà DataMashup della cartella di lavoro
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // Accedi alla raccolta PowerQueryFormulaParameters
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Itera attraverso i parametri per dimostrare FormulaDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Visualizza il valore della proprietà FormulaDefinition (proprietà di sola lettura)
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

                // Salva la cartella di lavoro
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

### Vedi anche

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


