---
title: "PowerQueryFormulaParameter.ParameterDefinition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaParameter-Eigenschaft. Gibt die Definition des Parameters zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

Liest die Definition des Parameters.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PowerQueryFormulaParameter.FormulaDefinition-Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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

                    // Iterieren Sie durch die Parameter, um ParameterDefinition zu demonstrieren
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Zeigen Sie den Wert der ParameterDefinition-Eigenschaft an (schreibgeschützte Eigenschaft)
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

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


