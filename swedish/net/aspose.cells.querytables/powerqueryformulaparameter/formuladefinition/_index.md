---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaParameter-egenskap. Hämtar definitionen av parametern"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Hämtar definitionen av parametern.

```csharp
public override string FormulaDefinition { get; }
```

### Exempel

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

                    // Iterera genom parametrarna för att demonstrera FormulaDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Visa värdet för egenskapen FormulaDefinition (skrivskyddad egenskap)
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

                // Spara arbetsboken
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

### Se även

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


