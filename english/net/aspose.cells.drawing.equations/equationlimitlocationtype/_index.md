---
title: Enum EquationLimitLocationType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.EquationLimitLocationType enum. Specifies the limit location on an operator
type: docs
url: /net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Specifies the limit location on an operator.

```csharp
public enum EquationLimitLocationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| UndOvr | `0` | Specifies that the limit is centered above or below the operator. |
| SubSup | `1` | Specifies that the limit is on the right side of the operator. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add an equation shape to the worksheet
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Get the equation paragraph and its first child
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Create a Nary equation node
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Set the limit location to SubSup (right side of operator)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Add some content to the equation
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // Change to UndOvr (centered above/below operator)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Save the workbook
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


