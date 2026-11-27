---
title: "PowerQueryFormulaParameter.ParameterDefinition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaParameter-egenskap. Hämtar definitionen av parametern"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/
---
## PowerQueryFormulaParameter.ParameterDefinition property

Hämtar definitionen av parametern.

```csharp
[Obsolete("Use PowerQueryFormulaParameter.FormulaDefinition property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ParameterDefinition { get; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PowerQueryFormulaParameter.FormulaDefinition. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

                    // Iterera genom parametrarna för att demonstrera ParameterDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Visa värdet för egenskapen ParameterDefinition (skrivskyddad egenskap)
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

                // Spara arbetsboken
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

### Se även

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


