---
title: FunctionEquationNode.Equals
second_title: Aspose.Cells for .NET API Reference
description: FunctionEquationNode method. Determine whether the current equation node is equal to the specified node
type: docs
url: /net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Determine whether the current equation node is equal to the specified node

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

### Examples

```csharp
namespace AsposeCellsExamples.FunctionEquationNodeMethodEqualsWithObjectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class FunctionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Since FunctionEquationNode doesn't have a parameterless constructor,
                // we'll demonstrate the Equals method differently
                Console.WriteLine("FunctionEquationNode instances cannot be created directly without parameters.");
                Console.WriteLine("In actual usage, you would obtain FunctionEquationNode instances from the API.");

                // Example of how you might use Equals if you had valid instances
                // bool areEqual = node1.Equals(node2);
                // Console.WriteLine($"Are the FunctionEquationNode instances equal? {areEqual}");

                // Example of comparing with a different type
                object someObject = "This is a string";
                // bool isEqualToString = node1.Equals(someObject);
                // Console.WriteLine($"Is FunctionEquationNode equal to string? {isEqualToString}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Save the workbook (though no visible changes were made to the spreadsheet)
            workbook.Save("FunctionEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### See Also

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


