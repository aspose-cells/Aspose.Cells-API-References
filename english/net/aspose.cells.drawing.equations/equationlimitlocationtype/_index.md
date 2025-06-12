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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a text box to contain the equation
            var textBox = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 300, 100);

            // Get the equation paragraph from the text box
            var equationNode = textBox.GetEquationParagraph();

            // Create a sum operator with limits
            var sumNode = equationNode.AddChild(EquationNodeType.NaryEquation);
            var limitLocationNode = sumNode.AddChild(EquationNodeType.Limit);
            limitLocationNode.AddChild(EquationNodeType.Base).AddChild(EquationNodeType.Text).ToLaTeX(); // Set text via LaTeX
            limitLocationNode.AddChild(EquationNodeType.Limit).AddChild(EquationNodeType.Text).ToLaTeX(); // Set text via LaTeX
            sumNode.AddChild(EquationNodeType.Base).AddChild(EquationNodeType.Text).ToLaTeX(); // Set text via LaTeX

            // Save the result
            workbook.Save("EquationLimitLocationTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


