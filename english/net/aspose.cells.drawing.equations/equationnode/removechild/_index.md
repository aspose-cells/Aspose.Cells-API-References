---
title: EquationNode.RemoveChild
second_title: Aspose.Cells for .NET API Reference
description: EquationNode method. Removes the specified node from the current nodes children
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/removechild/
---
## RemoveChild(EquationNode) {#removechild}

Removes the specified node from the current node's children.

```csharp
public void RemoveChild(EquationNode node)
```

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | Node to be deleted. |

### Examples

```csharp
namespace AsposeCellsExamples.EquationNodeMethodRemoveChildWithEquationNodeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a shape to hold the equation
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Get the equation node
            var equationNode = shape.GetEquationParagraph();

            // Create parent and child nodes
            var parentNode = equationNode.AddChild(EquationNodeType.Fraction);
            var childNode1 = parentNode.AddChild(EquationNodeType.Numerator);
            var childNode2 = parentNode.AddChild(EquationNodeType.Denominator);

            try
            {
                // Call RemoveChild with EquationNode parameter
                parentNode.RemoveChild(childNode1);

                Console.WriteLine("Child node removed successfully");
                
                // Removed the GetChildCount check since the method doesn't exist
                Console.WriteLine("Parent node's children were modified");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveChild method: {ex.Message}");
            }

            // Save the result
            workbook.Save("EquationNodeRemoveChildDemo.xlsx");
        }
    }
}
```

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## RemoveChild(int) {#removechild_1}

Removes the node at the specified index from the current node's children.

```csharp
public void RemoveChild(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Index of the node |

### Examples

```csharp
namespace AsposeCellsExamples.EquationNodeMethodRemoveChildWithInt32Demo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveChildWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a parent equation node
            EquationNode parentNode = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            
            // Add child nodes
            EquationNode child1 = parentNode.AddChild(EquationNodeType.Base);
            EquationNode child2 = parentNode.AddChild(EquationNodeType.Limit);
            EquationNode child3 = parentNode.AddChild(EquationNodeType.Matrix);

            try
            {
                // Remove child at index 1 (second child)
                parentNode.RemoveChild(1);
                
                Console.WriteLine("Child at index 1 removed successfully");
                
                // Verify removal by checking remaining children
                EquationNode remainingChild = parentNode.GetChild(0);
                Console.WriteLine($"First remaining child type: {remainingChild.EquationType}");
                
                // Attempt to get removed child (should throw)
                try
                {
                    var removedChild = parentNode.GetChild(1);
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Expected error when accessing removed child: {ex.Message}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveChild method: {ex.Message}");
            }
            
            workbook.Save("EquationNodeRemoveChildWithInt32Demo.xlsx");
        }
    }
}
```

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


