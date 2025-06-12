---
title: PowerQueryFormulaFunction.F
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaFunction property. Gets and sets the definition of function
type: docs
url: /net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Gets and sets the definition of function.

```csharp
public string F { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Load a workbook that contains existing Power Query formulas
            Workbook workbook = new Workbook("example.xlsx");
            
            // Access Power Query formulas collection
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Retrieve an existing function formula by name
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Cast to PowerQueryFormulaFunction to access F property
            if (formula is PowerQueryFormulaFunction function)
            {
                // Demonstrate getting the F property
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Demonstrate setting the F property
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


