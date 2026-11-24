---
title: "PowerQueryFormulaParameter.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaParameter-Eigenschaft. Gibt den Wert des Parameters zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Liest den Wert des Parameters.

```csharp
public string Value { get; set; }
```

### Beispiele

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

                    // Durchlaufen der Parameter, um die Value-Eigenschaft zu demonstrieren
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Den aktuellen Wert der Value-Eigenschaft anzeigen (Lesevorgang)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // Da Value les- und schreibbar ist, wird das Setzen eines neuen Werts demonstriert
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

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


