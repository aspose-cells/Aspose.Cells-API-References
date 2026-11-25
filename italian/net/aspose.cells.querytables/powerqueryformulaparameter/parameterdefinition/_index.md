---
title: "PowerQueryFormulaParameter.ParameterDefinition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaParameter. Ottiene la definizione del parametro"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

Ottiene la definizione del parametro.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PowerQueryFormulaParameter.FormulaDefinition. Questa proprietà sarà rimossa tra 12 mesi a partire da novembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

                    // Itera tra i parametri per dimostrare ParameterDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Visualizza il valore della proprietà ParameterDefinition (proprietà di sola lettura)
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

                // Salva la cartella di lavoro
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

### Vedi anche

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


