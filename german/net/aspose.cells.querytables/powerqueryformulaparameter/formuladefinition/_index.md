---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaParameter-Eigenschaft. Gibt die Definition des Parameters zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Liest die Definition des Parameters.

```csharp
public override string FormulaDefinition { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Greift auf die DataMashup‑Eigenschaft der Arbeitsmappe zu
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // Zugriff auf die PowerQueryFormulaParameters-Sammlung
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Iterieren Sie durch die Parameter, um FormulaDefinition zu demonstrieren
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Zeigen Sie den Wert der FormulaDefinition‑Eigenschaft an (schreibgeschützte Eigenschaft)
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

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


