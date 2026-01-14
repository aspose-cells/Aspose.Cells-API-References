---
title: Class PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormula class. Represents the definition of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Represents the definition of power query formula.

```csharp
public class PowerQueryFormula
```

## Properties

| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Gets the definition of the power query formula. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Gets the type of this power query formula. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Access the PowerQueryFormulas collection from DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Check if there are any existing formulas
                if (formulas.Count > 0)
                {
                    // Get the first PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // Display read-only properties
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Display and modify read-write properties
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Display the count of formula items
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Save the workbook
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormula: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


