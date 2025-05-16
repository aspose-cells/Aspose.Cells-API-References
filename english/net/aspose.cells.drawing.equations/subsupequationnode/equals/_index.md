---
title: SubSupEquationNode.Equals
second_title: Aspose.Cells for .NET API Reference
description: SubSupEquationNode method. Determine whether the current equation node is equal to the specified node
type: docs
url: /net/aspose.cells.drawing.equations/subsupequationnode/equals/
---
## SubSupEquationNode.Equals method

Determine whether the current equation node is equal to the specified node

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified node |

### Examples

```csharp
namespace AsposeCellsExamples.SubSupEquationNodeMethodEqualsWithObjectDemo
{
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class SubSupEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Create two SubSupEquationNode instances for comparison
                // Since SubSupEquationNode doesn't have a parameterless constructor,
                // we'll use the base class's constructor or create with minimal parameters
                SubSupEquationNode node1 = (SubSupEquationNode)Activator.CreateInstance(typeof(SubSupEquationNode), nonPublic: true);
                SubSupEquationNode node2 = (SubSupEquationNode)Activator.CreateInstance(typeof(SubSupEquationNode), nonPublic: true);
                
                // Compare the nodes using Equals method
                bool areEqual = node1.Equals((object)node2);
                
                // Display the comparison result
                Console.WriteLine($"Are the nodes equal? {areEqual}");
                
                // Compare with a different object type
                object differentObject = new object();
                bool areEqualWithObject = node1.Equals(differentObject);
                Console.WriteLine($"Is node equal to a generic object? {areEqualWithObject}");
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

* class [SubSupEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


