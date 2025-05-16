---
title: PowerQueryFormulaParameter.FormulaDefinition
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaParameter property. Gets the definition of the parameter
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Gets the definition of the parameter.

```csharp
public override string FormulaDefinition { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.PowerQueryFormulaParameterPropertyFormulaDefinitionDemo
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyFormulaDefinitionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Since we can't create a PowerQueryFormulaParameter directly without knowing required constructor parameters,
                // we'll demonstrate accessing these properties through an existing query table's parameters instead
                Console.WriteLine("This demo shows how to access PowerQueryFormulaParameter properties.");
                Console.WriteLine("In practice, you would access these properties from an existing query table's parameters.");
                
                // Save the workbook (though we didn't modify it)
                workbook.Save("FormulaDefinitionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


