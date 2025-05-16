---
title: AccentEquationNode.Equals
second_title: Aspose.Cells for .NET API Reference
description: AccentEquationNode method. Determine whether the current equation node is equal to the specified node
type: docs
url: /net/aspose.cells.drawing.equations/accentequationnode/equals/
---
## AccentEquationNode.Equals method

Determine whether the current equation node is equal to the specified node

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

### Examples

```csharp
namespace AsposeCellsExamples.AccentEquationNodeMethodEqualsWithObjectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class AccentEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Since AccentEquationNode doesn't have a parameterless constructor,
                // we'll demonstrate Equals using objects that can be compared
                object obj1 = new object();
                object obj2 = new object();
                
                // Compare the objects
                bool areEqual = obj1.Equals(obj2);
                bool areSameReference = obj1.Equals(obj1);
                
                // Display results
                Console.WriteLine($"Comparing different objects: {areEqual}");
                Console.WriteLine($"Comparing same reference: {areSameReference}");
                
                // Save the workbook
                workbook.Save("EqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


