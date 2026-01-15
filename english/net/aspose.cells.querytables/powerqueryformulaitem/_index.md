---
title: Class PowerQueryFormulaItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaItem class. Represents the item of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Represents the item of the power query formula.

```csharp
public class PowerQueryFormulaItem
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Gets the name of the item. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Gets the value of the item. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook (can be an existing file if you have Power Query data)
                Workbook workbook = new Workbook();

                // Access the DataMashup object which contains PowerQuery formulas
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Iterate through all PowerQuery formulas and their items
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Demonstrate read‑only Name property
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Demonstrate read/write Value property
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


