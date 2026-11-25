---
title: "PowerQueryFormulaParameter.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaParameter. Ottiene il valore del parametro"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Ottiene il valore del parametro.

```csharp
public string Value { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyValueDemo
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

                    // Itera tra i parametri per dimostrare la proprietà Value
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Visualizza il valore corrente della proprietà Value (operazione di lettura)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // Poiché Value è leggibile/scrivibile, dimostra l'impostazione di un nuovo valore
                        string newValue = "UpdatedValue_" + Guid.NewGuid().ToString();
                        parameter.Value = newValue;
                        Console.WriteLine($"Updated Value: {parameter.Value}");
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
                workbook.Save("ValueDemo.xlsx");
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


