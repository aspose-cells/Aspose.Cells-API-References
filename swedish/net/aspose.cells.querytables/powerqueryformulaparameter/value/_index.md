---
title: "PowerQueryFormulaParameter.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaParameter egenskap. Hämtar värdet av parametern"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Hämtar värdet av parametern.

```csharp
public string Value { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till DataMashup-egenskapen i arbetsboken
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // Åtkomst till PowerQueryFormulaParameters-samlingen
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Iterera genom parametrarna för att demonstrera Value-egenskapen
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Visa det aktuella värdet av egenskapen Value (läsläsning)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // Eftersom Value är läs/skriv, demonstrera att sätta ett nytt värde
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

                // Spara arbetsboken
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

### Se även

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


