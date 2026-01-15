---
title: PowerQueryFormula.Description
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets and sets the description of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Gets and sets the description of the power query formula.

```csharp
public string Description { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Load an existing file with Power Query formulas
                workbook = new Workbook("example.xlsx");

                // Access existing Power Query formulas
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Display the current Description value
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Set a new description
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Save the workbook
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


