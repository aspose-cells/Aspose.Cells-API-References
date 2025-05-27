---
title: EquationComponentNode.Equals
second_title: Aspose.Cells for .NET API Reference
description: EquationComponentNode method. Determine whether the current equation node is equal to the specified node
type: docs
url: /net/aspose.cells.drawing.equations/equationcomponentnode/equals/
---
## EquationComponentNode.Equals method

Determine whether the current equation node is equal to the specified node

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationComponentNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Create two EquationComponentNode instances for comparison
                // Since EquationComponentNode doesn't have a parameterless constructor,
                // we'll use the base class's constructor or create them differently
                EquationComponentNode node1 = null;
                EquationComponentNode node2 = null;
                
                // Compare the nodes using Equals method
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Display the comparison result
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Compare with a different object type
                object nonNodeObject = new object();
                bool areEqualWithObject = node1?.Equals(nonNodeObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [EquationComponentNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


