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
namespace AsposeCellsExamples
{
    using Aspose.Cells.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class SubSupEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                //test get mathnode
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                string[] vals = new string[] { "A", "B", "C" };
                int[] vs = null;
                EquationNode node = null;
                for (int i = 0; i < 4; i++)
                {
                    switch (i)
                    {
                        case 0:
                            node = mathNode.AddChild(EquationNodeType.Sub);
                            vs = new int[2] { 0, 1 };
                            break;
                        case 1:
                            node = mathNode.AddChild(EquationNodeType.Sup);
                            vs = new int[2] { 0, 2 };
                            break;
                        case 2:
                            node = mathNode.AddChild(EquationNodeType.SubSup);
                            vs = new int[3] { 0, 1, 2 };
                            break;
                        case 3:
                            node = mathNode.AddChild(EquationNodeType.PreSubSup);
                            vs = new int[3] { 1, 2, 0 };
                            break;
                    }

                    foreach (var v in vs)
                    {
                        switch (v)
                        {
                            case 0:
                                EquationNode e = node.AddChild(EquationNodeType.Base);
                                TextRunEquationNode TR = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
                                TR.Text = vals[v];
                                break;
                            case 1:
                                EquationNode sub = node.AddChild(EquationNodeType.Subscript);
                                TR = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
                                TR.Text = vals[v];
                                break;
                            case 2:
                                EquationNode sup = node.AddChild(EquationNodeType.Superscript);
                                TR = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
                                TR.Text = vals[v];
                                break;
                        }
                    }
                }

                SubSupEquationNode node1 = (SubSupEquationNode)mathNode.GetChild(0);
                SubSupEquationNode node2 = (SubSupEquationNode)mathNode.GetChild(1);           
                

                // Compare the nodes using Equals method
                bool areEqual = node1.Equals((object)node2);
                
                // Display the comparison result
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Compare the nodes using Equals method
                areEqual = node1.Equals((object)node1);

                // Display the comparison result
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Compare with a different object type
                object differentObject = new object();
                bool areEqualWithObject = node1.Equals(differentObject);
                Console.WriteLine($"Is node equal to a generic object? {areEqualWithObject}");

                workbook.Save("SubSupEquationNodeMethodEqualsWithObjectDemo.xlsx");
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


